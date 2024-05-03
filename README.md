'docker-compose.yml' for nginx-proxy with acme-companion.

It works for multiple domains with one nginx server through 'SNI' protocol.

You need to create network for proxy.

exec below commands in order.

1. exec 'sudo docker network create nginx-proxy-network'
2. exec 'docker-compose up -d'

..then build service with nginx-proxy served environment options.
Check the sample docker-compose file for service in 'app' folder.
(expose port option must be declared)

special thanks to 'https://github.com/nginx-proxy'
