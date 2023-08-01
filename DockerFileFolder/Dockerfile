# Use the official Apache image as the base image
FROM httpd:2.4

# Set the working directory in the container
WORKDIR /usr/local/apache2/htdocs

# Copy your static webpage files from the local directory to the container's working directory
COPY ./index.html /usr/local/apache2/htdocs/

# Expose the port that Apache will listen on (usually port 80)
EXPOSE 80

# The CMD instruction defines the default command that will be executed when the container starts.
CMD ["httpd", "-D", "FOREGROUND"]
