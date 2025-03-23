# Use the official Node.js latest image as the base image
FROM node:latest

# Set the working directory inside the container
WORKDIR /app

# Copy package.json and package-lock.json to the working directory
COPY package*.json ./

# Install production dependencies
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port your app runs on (e.g., 3000)
EXPOSE 8080

# Define the command to run your application
CMD ["node", "index.js"]
