# Use official Node.js image
FROM node:18-alpine

# Set working directory
WORKDIR /app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy application source code
COPY target/database_service_project-*.jar app.jar

# Expose application port
EXPOSE 3000

# Start the application
CMD ["npm", "start"]
