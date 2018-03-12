# nginx-proxy-compose
Starter project for serving your node web app with nginx acting as a reverse proxy to your node api and your nginx web server with ssl enabled using the following containers.

- jwilder/nginx-proxy
- jrcs/letsencrypt-nginx-proxy-companion
- node
- mongo

Make sure your server allow port 80 for http and 443 for https

# Usage
1. Put your node api code in ./node-api/code
2. Put your www code in ./www/public
3. Run docker volume create nginxcerts mongodbdata
4. Run docker-compose build
5. Run docker-compose up -d
6. Run docker-compose down -v

# Contribution
Yes, please.
