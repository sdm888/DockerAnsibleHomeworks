FROM nginx:1.27-alpine

RUN apk add --no-cache curl

ADD ./default.conf /etc/nginx/config
ADD ./index.html /usr/share/nginx/html

EXPOSE 80
