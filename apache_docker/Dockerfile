FROM httpd:2.4-alpine

RUN apk update; apk upgrade

# Copy virtual host file
COPY httpd-vhosts.conf /usr/local/apache2/conf/httpd-vhosts.conf
RUN echo "Include /usr/local/apache2/conf/httpd-vhosts.conf" \
    >> /usr/local/apache2/conf/httpd.conf