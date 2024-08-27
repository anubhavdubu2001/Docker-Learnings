# Use the official Python base image
FROM python:3.12-slim

# Set the working directory
WORKDIR /app

# Copy the requirements file and devops directory into the container
COPY requirements.txt /app
COPY devops /app

# Install the required Python packages
RUN pip install --no-cache-dir -r requirements.txt

# Set the entry point and default command
ENTRYPOINT ["python3"]
CMD ["manage.py", "runserver", "0.0.0.0:8000"]

