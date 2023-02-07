# Use an official Python image as the base image
FROM python:3.9-alpine

RUN mkdir /app
ADD . /app

# Set the working directory in the container
WORKDIR /app
RUN pip install flask
RUN pip freeze > requirements.txt
RUN pip install -r requirements.txt
EXPOSE 5000
# Run the Flask application
CMD ["python", "hello.py"]
