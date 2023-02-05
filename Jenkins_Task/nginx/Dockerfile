FROM ubuntu:latest
RUN apt-get update && apt-get install nginx -y
ARG W
COPY index.html /var/www/html/
RUN cat /var/www/html/index.html
CMD ["nginx", "-g", "daemon off;"]
