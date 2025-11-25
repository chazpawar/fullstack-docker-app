# Use Node.js 14 Alpine as base image (lightweight)
FROM node:14-alpine

# Set working directory inside container
WORKDIR /app

# Copy package.json first (for better caching)
COPY package.json .

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the port the app runs on
EXPOSE 5000

# Command to start the application
CMD ["npm", "start"]