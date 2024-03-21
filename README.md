# Custom Caddy build

This is building on the serfriz/caddy-custom-build images provided by serfriz. I wanted to start learning how to create and maintain these images and use other modules for my own use.

This image is updated automatically by GitHub Actions when a new version of Caddy is released using the official Caddy Docker image and the following modules:

- [**Cloudflare DNS:**](https://github.com/caddy-dns/cloudflare) for Cloudflare DNS-01 ACME validation support | caddy-dns/cloudflare 
- [**Cloudflare IPs:**](https://github.com/WeidiDeng/caddy-cloudflare-ip) to retrieve Cloudflare's current IP ranges | WeidiDeng/caddy-cloudflare-ip 
- [**Dynamic DNS:**](https://caddyserver.com/docs/modules/dynamic_dns) updates the DNS records with the public IP address of your instance | mholt/caddy-dynamicdns 
- [**CrowdSec Bouncer:**](https://github.com/hslatman/caddy-crowdsec-bouncer) to blocks malicious traffic based on CrowdSec decisions | hslatman/caddy-crowdsec-bouncer 
- [**MaxMind Geolocation:**](https://github.com/porech/caddy-maxmind-geolocation) to allow or block traffic from specific regions based on maxmind geo database | porech/caddy-maxmind-geolocation


## **Usage**

Since this image built off the official Caddy Docker image, the same volumes and/or bind mounts, ports mapping, etc. can be used with this container. 
Additional environment variables may be needed for the added modules. Please, refer to the repository's README file for further usage instructions.


## Docker builds available at the following container registries:

- **Docker Hub** docker pull Rupie17/caddy-cf-ddns-csec-geoip:latest 


## **Tags** 
The following tags are available for the Rupie17/caddy-cf-ddns-crowdsec-geoip image:

latest (eg: 2.7.4, including: 2.7, 2, etc.)


## **Contributing**
Feel free to contribute, request additional Caddy images with your preferred modules, and make things better by opening an Issue or Pull Request.


## **License**
Software under GPL-3.0 ensures users' freedom to use, modify, and distribute it while keeping the source code accessible. It promotes transparency, collaboration, and knowledge sharing. Users agree to comply with the GPL-3.0 license terms and provide the same freedom to others.
