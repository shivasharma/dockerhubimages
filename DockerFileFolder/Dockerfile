
# Use a base image, preferably a lightweight web server
# For a static webpage, we'll use nginx as an example
FROM nginx:alpine

# Set the working directory to /usr/share/nginx/html
WORKDIR /usr/share/nginx/html

# Copy the static website files from your local machine to the container's working directory
COPY ./index.html/ .

# Expose port 80 to allow incoming HTTP traffic
EXPOSE 80

# Start the web server when the container is launched
CMD ["nginx", "-g", "daemon off;"]
