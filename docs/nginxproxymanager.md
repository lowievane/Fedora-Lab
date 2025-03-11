# Nginx Proxy Manager

> [Docker Compose file](../stacks/nginxproxymanager.yaml)

I use Nginx Proxy Manager as a reverse proxy with SSL certificates. This way I can setup subdomains for every application running in the homelab, all secured by the certificate and available over the HTTPS protocol. I've set this up by pointing my domain to the local IP of the Nginx Proxy Manager instance. This way the domain will only work when I'm connected to my own network, which makes it very secure. I then requested the SSL certificate for both my domain and all possible subdomains, and eventually I configured the subdomains so every application redirects correctly.
