# Use an official Node.js runtime as a parent image
FROM node:14-alpine

# Set the working directory to /app
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Install any necessary dependencies
RUN npm install

# Build the React app
RUN npm run build

# Expose port 80 for the web server
EXPOSE 3000

# Start the web server
CMD ["npm", "start"]

