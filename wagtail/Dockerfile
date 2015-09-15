# Use the official nginx build
FROM nginx:latest

MAINTAINER Marko Kirves <marko.kirves@bynd.com>

# Disable default site
RUN rm /etc/nginx/conf.d/default.conf

# Create cache directory
RUN mkdir -p /var/cache/nginx

# Add application configuration
ADD wagtail-app.conf /etc/nginx/conf.d/wagtail-app.conf

# Use volume for cache directory
VOLUME ["/var/cache/nginx"]
