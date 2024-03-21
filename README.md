This is building on the serfriz/caddy-custom-build images provided by serfriz. I wanted to start learning how to create and maintain these images and use other modules for my own use.

This image is updated automatically by GitHub Actions when a new version of Caddy is released using the official Caddy Docker image and the following modules:

**Cloudflare DNS:** for Cloudflare DNS-01 ACME validation support | caddy-dns/cloudflare 
**Cloudflare IPs:** to retrieve Cloudflare's current IP ranges | WeidiDeng/caddy-cloudflare-ip 
**Dynamic DNS:** updates the DNS records with the public IP address of your instance | mholt/caddy-dynamicdns 
**CrowdSec Bouncer:** to blocks malicious traffic based on CrowdSec decisions | hslatman/caddy-crowdsec-bouncer 
**MaxMind Geolocation:** to allow or block traffic from specific regions based on maxmind geo database | caddy-maxmind-geolocation

**Usage**

Since this image built off the official Caddy Docker image, the same volumes and/or bind mounts, ports mapping, etc. can be used with this container. 
Additional environment variables may be needed for the added modules. Please, refer to the repository's README file for further usage instructions.

Docker builds for all Caddy supported platforms available at the following container registries:

**Docker Hub** docker pull Rupie17/caddy-cloudflare-ddns-crowdsec:latest 
**GitHub Packages** docker pull ghcr.io/serfriz/caddy-cloudflare-ddns-crowdsec:latest

**Tags** 
The following tags are available for the Rupie17/caddy-cf-ddns-crowdsec-geoip image:

latest (eg: 2.7.4, including: 2.7, 2, etc.)

**Contributing**
Feel free to contribute, request additional Caddy images with your preferred modules, and make things better by opening an Issue or Pull Request.

**License **
Software under GPL-3.0 ensures users' freedom to use, modify, and distribute it while keeping the source code accessible. It promotes transparency, collaboration, and knowledge sharing. Users agree to comply with the GPL-3.0 license terms and provide the same freedom to others.
