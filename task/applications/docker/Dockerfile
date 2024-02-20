# Official Python image for the base
FROM python:3.9-slim

#The working directory in the container
WORKDIR /app

#Copying the current working directory contents into the container at /app
COPY . /app

#Installing dependencies reequired by the application
RUN pip install --no-cache-dir flask

#Exposing the PORT on which flask will run
EXPOSE 2024

# Define environment variable
ENV FLASK_APP=hello.py

#Command to run the flask application
CMD ["flask", "run", "--host=0.0.0.0", "--port=2024"]