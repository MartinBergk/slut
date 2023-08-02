# Use an official Python runtime as the base image
FROM python:3.8

# Install MongoDB client
RUN apt-get update && apt-get install -y mongodb-clients

# Set the working directory in the container
WORKDIR /app

# Copy requirements.txt to the working directory
COPY requirements.txt ./

# Install backend dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy all files to the container's working directory
COPY . .

# Set the command to start the backend
CMD ["python", "app.py"]
