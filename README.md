


A complimentry setup for using Shadowsocks client to access your content remotely while utilizing pi-hole for DNS.

Shadowsocks Server:


Pi-hole Server (filtering DNS):

SERVER_IP=255.255.255.255
WEBPASSWORD="PiHoleAdminPassword"
VIRTUAL_HOST="admin-access.pihole.com"
PROXY_PASSWORD=YourComplicatedPassword

    image: diginc/pi-hole:alpine
      IPv6: "False"
    volumes:
      - "./pihole/:/etc/pihole/"
      - "./dnsmasq.d/:/etc/dnsmasq.d/"
    ports:
      - "89:80/tcp"

    image: vimagick/shadowsocks-libev
  
<iframe src="https://www.vpnmentor.com/blog/shadowsocks-vs-vpns-everything-need-know/"> </iframe>
