FROM nginx:1.27.2

COPY nginx/default.conf /etc/nginx/conf.d/

COPY nginx/html /var/www/html

WORKDIR /var/www

RUN touch /var/run/nginx.pid && \
chown -R nginx:nginx /var/run/nginx.pid && \
chown -R nginx:nginx /var/cache/nginx

USER nginx
