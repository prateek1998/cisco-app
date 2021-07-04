# Setup Steps to Follow

1. Run the command to build your docker.
```bash 
docker-compose build
```
2. Run the command to run your docker in background.
```bash 
docker-compose up -d
```
3. Now you will see, there are two different container will start.
4. Now copy the docker container name ending with name nginx.
for example:
`cisco-app_nginx_1`
5. Copy this container name and then use this command and to go inside the container.
```bash 
docker exec -it cisco-app_nginx_1 bash
```
6. Now you are inside the container, run this command including your domain name.
```bash
certbot --nginx -d ackmyconfig.com -d www.ackmyconfig.com
```
7. press 'y' to generate ssl certificate.
