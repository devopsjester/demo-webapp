# Use the official latest Python image from Docker Hub
FROM python:latest

# Create a new user "vscode"
RUN useradd -m vscode

# Change to the new user
USER vscode

# Set the working directory to /app in the container
WORKDIR /app

# Add the current directory contents to the container at /app
ADD . /app

# Install any needed packages specified in requirements.txt
RUN pip install --no-cache-dir -r requirements.txt

# Make port 5000 available for the app
EXPOSE 5000

# Run the application
CMD ["python", "app.py"]
