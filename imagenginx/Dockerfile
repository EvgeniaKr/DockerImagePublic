FROM nginx:1.20

COPY ./nginx.conf /etc/nginx/nginx.conf
COPY ./moduls /etc/nginx/moduls
COPY ./certs/ /etc/nginx/certs


RUN chown -R nginx:nginx /var/cache/nginx && \
        chown -R nginx:nginx /var/log/nginx && \
        chown -R nginx:nginx /etc/nginx/ && \
        touch /var/run/nginx.pid && \
        chown -R nginx:nginx /var/run/nginx.pid 

USER nginx

EXPOSE 80 443

