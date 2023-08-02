# Use the official Node.js image
FROM node:latest

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files to the container
COPY package*.json ./

# Install frontend dependencies
RUN npm install

# Copy all frontend source code to the container
COPY . .

# Build the frontend app
RUN npm run build

# Set the command to start the frontend server
CMD [ "npm", "start" ]
