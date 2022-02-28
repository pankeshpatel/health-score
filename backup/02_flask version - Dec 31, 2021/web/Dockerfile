# Pull an image with python and base image
FROM python:3

WORKDIR /usr/src/app

# Install all packages (mentioned in requirements.txt) into container
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# Copy all files (app.py, MD04 folder) from current folder to the container
COPY . .

# Run the command
CMD ["python", "app.py"]