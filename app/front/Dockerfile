FROM nginx:latest

ENV WS_BACK_URL=http://localhost:8080

WORKDIR /usr/share/nginx/html

RUN rm -rf ./*

COPY ./front /usr/share/nginx/html

COPY ./front/entrypoint.sh /entrypoint.sh

RUN chmod +x /entrypoint.sh

ENTRYPOINT ["/entrypoint.sh"]

EXPOSE 80

