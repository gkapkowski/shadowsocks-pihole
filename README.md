Secure Ad Free Browsing docker-compose
======================================

A complimentry setup for using Shadowsocks client to access your content remotely while utilizing pi-hole for DNS.

#### What is/Why ShadowSocks?
https://qz.com/1072701/meet-shadowsocks-the-underground-tool-that-chinas-coders-use-to-blast-through-the-great-firewall/
https://www.vpnmentor.com/blog/shadowsocks-vs-vpns-everything-need-know/

#### What is/Why Pi-Hole?
https://pi-hole.net/2017/05/12/seven-things-you-may-not-know-about-pi-hole/
https://discourse.pi-hole.net/t/why-should-pi-hole-be-my-only-dns-server/3376


YOU ----> Local ShadowSocks Client
                   |
            ssh over internet
                   |
           Shadow Socks Server ----- check if "BAD" address -> YES -> return nothing
                   |<-----lookup DNS from google as normal <- NO
                   |
             get  <|> content
              from Internet
              
### Net Result : 
    Your content delivered to your local machine over a secure encrypted connection 
    Your content has been stripped of Ad domains etc so its faster and smaller
    
### And why is that good : 
    Because you look at more porn than anyone and advertisers thought it was easier for you to block them.
    Sorry dude. 
    nah - ad's suck ass - snooping sucks ass - your mom.....


to-do
* finish readme
* credit sources
* speed comparisons
