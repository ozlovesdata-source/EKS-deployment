# Use a lightweight Linux base image (Alpine)
FROM alpine:3.20

# Set the working directory inside the container
WORKDIR /app

# Install dependencies (e.g., Python3 and pip)
# 'apk' is the Alpine package manager
RUN apk add --no-cache python3 py3-pip

# Copy your backend application code into the container
# The first '.' is your local code, the second '.' is the WORKDIR (/app)
COPY . .

# (Optional) Install your app's Python requirements
# RUN pip install -r requirements.txt

# Tell Docker what port your application will run on
EXPOSE 8080

# The command to run when the container starts
# This example assumes you have a 'main.py' file
CMD ["python3", "main.py"]
