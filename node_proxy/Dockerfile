# Set the base image to Ubuntu
FROM ubuntu

# File Maintainer
MAINTAINER Mathieu Gamache

# Install Node.js and other dependencies
RUN apt-get update && \
    apt-get -y install curl && \
    curl sL https://deb.nodesource.com/setup | sudo bash - && \
    apt-get -y install python build-essential nodejs

# Install nodemon (http://nodemon.io/)
#RUN npm install -g nodemon

# Copy the files from the host to the images
COPY ./src /var/src

# Install the dependencies
RUN cd /var/src;  npm install

EXPOSE 8000

CMD ["node", "/var/src/index.js"]
