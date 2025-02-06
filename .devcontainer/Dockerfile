# Use a base image with Python 3.10
FROM mcr.microsoft.com/devcontainers/python:3.10

# Set the working directory
WORKDIR /workspace

# Install essential Python packages
RUN apt-get update && apt-get install -y \
    python3-pip python3-venv python3-dev \
    && rm -rf /var/lib/apt/lists/*

# Upgrade pip and install common dependencies
RUN pip install --no-cache-dir --upgrade pip setuptools wheel

# Set default shell to bash
SHELL ["/bin/bash", "-c"]