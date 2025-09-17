# Base image
FROM ubuntu:latest

# Update and upgrade
RUN apt-get update && apt-get upgrade -y

# Install python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix externally managed Python issue (if needed)
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask via pip3
RUN pip3 install flask

RUN pip3 install flask flask-cors

# Set working directory
WORKDIR /app

# Copy the API script into the container
COPY ./api.py /app/api.py

# Command to run Flask app
CMD ["python3", "api.py"]

