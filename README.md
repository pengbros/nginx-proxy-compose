# nginx-proxy-compose
Starter project for serving your node web app with nginx acting as a reverse proxy to your node api and your nginx web server, all with ssl enabled. The starter project leverages the following containers. 

- jwilder/nginx-proxy
- jrcs/letsencrypt-nginx-proxy-companion
- node
- mongo

For detailed configurations, consult the readme of each containers. Please also make sure your server allow connections on port 80 for http and 443 for https.

# Usage
1. Put your node api code in ./node-api/code
2. Put your www code in ./www/public
3. Edit docker-compose.yml and ./node-api/Dockerfile
4. Run docker volume create nginxcerts mongodbdata
5. Run docker-compose build
6. Run docker-compose up -d
7. Run docker-compose down -v

# Contribution
Yes, please.

# License
[MIT License](https://opensource.org/licenses/mit-license.php)
