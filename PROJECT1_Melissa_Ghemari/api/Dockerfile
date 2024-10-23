# Use a lightweight Python image
FROM python:3.9-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the API source code into the container
COPY . /app

# Install the dependencies listed in requirements.txt
RUN pip install -r requirements.txt

# Expose port 8080, which the FastAPI app will run on inside the container
EXPOSE 8080

# Command to run the FastAPI app when the container starts
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8080"]
