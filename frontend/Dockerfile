# Use the official lightweight Nginx image
FROM nginx:1.27-alpine-slim

# Set the working directory
WORKDIR /usr/share/nginx/html

# Clean out the default Nginx welcome page
RUN rm -rf ./*

# Copy your built frontend code (e.g., from a 'build' or 'dist' folder)
# This path './build' is relative to where the Dockerfile is.
COPY ./build .

# Nginx listens on port 80 by default
EXPOSE 80

# The Nginx base image already includes a CMD, so you don't need one.
