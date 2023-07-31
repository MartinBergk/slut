# Use an official Node.js runtime as the base image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy the rest of the frontend source code to the container
COPY . .

# Build the frontend
RUN npm run build

# Expose the port your frontend is running on (e.g., 3000)
EXPOSE 3000

# Define the command to start your frontend application
CMD ["npm", "start"]
