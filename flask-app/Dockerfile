# Use python:3.9-slim as the base image
FROM python:3.9-slim

# Set the working directory
WORKDIR /app

# Copy requirements and install dependencies
COPY requirement.txt .
RUN pip install --no-cache-dir -r requirement.txt

# Copy application code
COPY . .

# Expose the application port
EXPOSE 5000

# Set the entrypoint
CMD ["python", "main.py"]
