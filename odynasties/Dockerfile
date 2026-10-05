FROM php:8.2-apache

# Install the extensions PHP needs to talk to MySQL
RUN docker-php-ext-install pdo pdo_mysql

# Enable URL rewriting for Apache
RUN a2enmod rewrite

# Copy your code into the web server directory
COPY . /var/www/html/
WORKDIR /var/www/html
EXPOSE 80
