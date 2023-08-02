# Use the official NGINX image as the base image
FROM nginx

# Remove default NGINX configurations
RUN rm /etc/nginx/conf.d/default.conf

# Copy custom NGINX configuration to the container's NGINX configuration directory
COPY nginx.conf /etc/nginx/nginx.conf

# Expose port 80
EXPOSE 80

