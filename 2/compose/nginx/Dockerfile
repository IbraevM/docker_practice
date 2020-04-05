FROM alpine:3.11.5

RUN apk add --no-cache nginx && mkdir -p /run/nginx

EXPOSE 80

COPY custom.conf /etc/nginx/conf.d/

COPY ./www/ /var/www/ 

CMD ["nginx", "-g", "daemon off;"]
