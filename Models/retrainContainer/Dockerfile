# Use an official Python runtime as a parent image
FROM python:3.5.2

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Make port 6006 available to the world outside this container
EXPOSE 5000
EXPOSE 80
EXPOSE 6006

# Define environment variable
ENV NAME World

# Run app.py when the container launches
CMD ["python", "app.py"]