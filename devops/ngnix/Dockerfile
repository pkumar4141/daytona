FROM nginx
RUN rm /etc/nginx/conf.d/default.conf
COPY nginx.conf /etc/nginx/conf.d/default.conf
RUN mkdir -p /var/www/html/errors
COPY 404.html /var/www/html/errors
COPY 50x.html /var/www/html/errors
