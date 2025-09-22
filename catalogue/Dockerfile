
FROM node:20-alpine3.21
WORKDIR /opt/server
COPY package.json .
COPY *.js .
RUN npm install 
ENV MONGO="true" \
    MONGO_URL="mongodb://mongodb:27017/catalogue"
CMD ["node","server.js"]













# chown: Changes file or directory ownership.

# -R: Applies the change recursively to all files and subfolders.

# roboshop:roboshop: Sets the user and group to "roboshop".

# /opt/server: Specifies the target directory.
# This command gives full ownership of /opt/server and everything inside it to the user and group named "roboshop".