# Use an official Node.js runtime as the base image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install backend dependencies
RUN npm install

# Copy the rest of the backend source code to the container
COPY . .

# Expose the port your backend is running on (e.g., 5000)
EXPOSE 5000

# Define the command to start your backend application
CMD ["npm", "start"]
