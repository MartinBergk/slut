# Use an official Python runtime as the base image
FROM python:3.8

# Install MongoDB client
RUN apt-get update && apt-get install -y mongodb-clients

# Set the working directory in the container
WORKDIR /app

# Copy backend files from the 'server' directory
COPY server/ ./

# Install backend dependencies using environment variables
ENV MONGO_URL="mongodb+srv://martinbergkvist13:campus09@test.yy3xqvh.mongodb.net/?retryWrites=true&w=majority"

# Install backend dependencies
RUN pip install --no-cache-dir pymongo flask

# Set the command to start the backend
CMD ["python", "app.py"]

