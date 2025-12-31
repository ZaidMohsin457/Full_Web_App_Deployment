# Use the official Python 3.12 slim image (Lightweight and secure)
FROM python:3.12-slim

# Set the working directory inside the container
WORKDIR /app

# Copy the requirements file first (for better caching)
COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Copy the rest of the application code
COPY . .

# Expose port 5000 to the outside world
EXPOSE 5000

# Command to run the application
CMD ["python", "main.py"]
