# Use the official Node.js image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install backend dependencies
RUN npm install

# Copy all backend source code to the container
COPY . .

# Set the command to start the backend server
CMD [ "npm", "start" ]



