# Use an official Node runtime as the base image
FROM node:14

# Set the working directory in the container
WORKDIR /app

# Copy frontend files from the 'public' directory
COPY public/ ./

# Install frontend dependencies
RUN npm install

# Build the frontend
RUN npm run build

# Set the command to start the frontend
CMD ["npm", "start"]
