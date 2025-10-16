# Python Web App

A simple Python web application that returns "Hello World." Built with Flask and containerized with Docker for easy deployment.

## Features

- Simple Flask web application
- Returns "Hello World." on the root endpoint
- Health check endpoint at `/health`
- Fully containerized with Docker
- Production-ready configuration

## How to Use

**Build the Docker image:**
```bash
docker build -t python-web-app .
```

**Run the container:**
```bash
docker run -p 8080:5000 python-web-app
```

**Test the application:**
```bash
curl http://localhost:8080
# Returns: Hello World.

curl http://localhost:8080/health
# Returns: {"status": "healthy"}
```

## Project Structure

- `app.py` - Main Flask application
- `requirements.txt` - Python dependencies
- `Dockerfile` - Docker configuration
- `.dockerignore` - Docker build optimization