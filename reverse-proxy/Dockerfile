FROM nginx:alpine

COPY ./conf/default.conf.template /etc/nginx/conf.d/default.conf.template

CMD /bin/sh -c "envsubst < /etc/nginx/conf.d/default.conf.template > /etc/nginx/nginx.conf && nginx -g 'daemon off;'"

EXPOSE 80