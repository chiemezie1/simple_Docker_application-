# Use an official Node.js runtime as the base image
FROM node

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the application files to the working directory
COPY . .

# Expose port 3000 for the application
EXPOSE 4000

# Use nodemon to run the application
CMD ["npx", "nodemon", "--exec", "babel-node", "index.js"]