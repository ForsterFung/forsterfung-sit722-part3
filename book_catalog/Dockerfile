# Your Solution
# Dockerfile for book_catalog microservice

# Use an official Python runtime as a parent image
FROM python:3.9-slim

# Root Directory
WORKDIR /book_catalog

# Copies the source code for this microservice into the image
COPY ./* .

# Set Environment Variable
ENV DATABASE_URL=postgresql://devopsprojectpart3_user:YVN7Ez95qwWGIGl0uUiAiCSOdBplax0F@dpg-cr6n8a56l47c7396k8ig-a.oregon-postgres.render.com/devopsprojectpart3

# Build Command
RUN pip install -r requirements.txt

# Start command
CMD uvicorn main:app --host 0.0.0.0 --port $PORT