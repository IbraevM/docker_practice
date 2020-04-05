FROM debian

COPY . /opt/

RUN apt-get update
RUN apt-get install -y nginx

COPY custom.conf /etc/nginx/conf.d/

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
