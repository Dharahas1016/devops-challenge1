# Use an official Nginx image as a base image
FROM nginx:latest

# Copy the contents of the frontend directory to the default Nginx public directory
COPY . /usr/share/nginx/html

# Expose port 80 to the outer world
EXPOSE 80

# Command to start Nginx when the container starts
CMD ["nginx", "-g", "daemon off;"]

