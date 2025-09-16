# Use nginx image
FROM nginx:latest

# Copy front-end files to nginx html directory
COPY ./softy-pinko-front-end /var/www/html/softy-pinko-front-end

# Copy custom nginx config
COPY ./softy-pinko-front-end.conf /etc/nginx/conf.d/default.conf