# Use Node.js 14 Alpine as base image
FROM node:14-alpine

# Set working directory
WORKDIR /app

# Copy package.json
COPY package.json .

# Install dependencies
RUN npm install

# Copy the rest of the application
COPY . .

# Expose port 3000
EXPOSE 3000

# Start the React development server
CMD ["npm", "start"]