# Use an official Python runtime as the base image
FROM python:3.9

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any needed dependencies specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 2024 available to the world outside this container
EXPOSE 2024

# Define environment variable
#ENV set FLASK_APP="hello.py"

ENV export FLASK_APP="hello.py"

# Run hello.py when the container launches
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0"]

