# Use the official Python image from the Docker Hub
FROM python:3.9

# Set the working directory in the container
WORKDIR /app

# Install required dependencies
RUN pip3 install fastapi
RUN pip3 install "uvicorn[standard]"

# Copy the entire current directory into the container at /app
COPY . .

# Expose the port that your FastAPI application runs on (default is 8000)
EXPOSE 8000

# Command to run the FastAPI application within the container
CMD ["uvicorn", "api:app", "--host", "0.0.0.0", "--port", "8000"]

