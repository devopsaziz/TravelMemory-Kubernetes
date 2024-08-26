# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy package.json and package-lock.json (if available)
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of your application code to the container
COPY . .

# Expose the port the app runs on
EXPOSE 3001

# Command to run the application
CMD ["node", "index.js"]
