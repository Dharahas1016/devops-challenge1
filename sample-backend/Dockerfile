# Use an official Python image as a base image
FROM python:3.8

# Set the working directory in the container
WORKDIR /app

# Copy the backend files to the container
COPY . /app


# Install uvicorn
RUN pip install uvicorn
# Install any needed packages specified in requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Expose the port the app runs on
EXPOSE 8000

# Command to run the application
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]

