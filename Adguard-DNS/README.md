# Adguard DNS

## Introduction

AdGuard Home is a network-wide software for blocking ads and tracking. After you set it up, it'll cover all your home devices, and you won't need any client-side software for that. Learn more on our official Github repository.

## Ports mappings you may need:

-p 53:53/tcp -p 53:53/udp: 
  - plain DNS.

-p 67:67/udp -p 68:68/tcp -p 68:68/udp: 
   - add if you intend to use AdGuard Home as a DHCP server.

-p 80:80/tcp -p 443:443/tcp -p 443:443/udp -p 3000:3000/tcp: 
  - add if you are going to use AdGuard Home's admin panel as well as run AdGuard Home as an HTTPS/DNS-over-HTTPS server.

-p 853:853/tcp: 
  - add if you are going to run AdGuard Home as a DNS-over-TLS server.

-p 784:784/udp -p 853:853/udp -p 8853:8853/udp: 
  - add if you are going to run AdGuard Home as a DNS-over-QUIC server. You may only leave one or two of these.

-p 5443:5443/tcp -p 5443:5443/udp: 
  - add if you are going to run AdGuard Home as a DNSCrypt server.

## URL
- https://adguard.com/en/welcome.html
- https://github.com/AdguardTeam/AdGuardHome
- https://hub.docker.com/r/adguard/adguardhome