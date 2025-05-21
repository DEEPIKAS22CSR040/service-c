# Use official Python image as base
FROM python:3.9-slim

# Set working directory
WORKDIR /app

# Copy requirements.txt if you have one, else install flask directly
RUN pip install flask

# Copy app files
COPY app.py .

# Copy tests folder (optional if you want tests inside container)
COPY tests ./tests

# Expose port
EXPOSE 5000

# Command to run the app
CMD ["python", "app.py"]
