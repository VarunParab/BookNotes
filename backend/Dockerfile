# Use an official Node.js runtime as a base image
FROM node:14-alpine

# Set the working directory to /app
WORKDIR /app/backend

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the content of the local src directory to the working directory
COPY . .

# Expose port 5000
EXPOSE 5000

# Start the backend application
CMD ["npm", "start"]
