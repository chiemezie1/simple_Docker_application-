# Use an official Node.js runtime as the base image
FROM node

# Set the working directory inside the container
WORKDIR /client

# Copy package.json and package-lock.json to the working directory
COPY package*.json /client

# Install app dependencies
RUN npm install

# Copy the rest of the application files to the working directory
COPY .  /client/

# Expose port 3000 for the application
EXPOSE 3000

# Use nodemon to run the application
CMD ["npm", "start"]

