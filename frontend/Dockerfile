# Use an official Node.js runtime as a parent image
FROM node:18

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json to the working directory
COPY package*.json ./

# Install any needed packages
RUN npm install

# Copy the rest of the application code to the working directory
COPY . .

# Expose the port that your app will run on
EXPOSE 3000

# Command to run the application
CMD ["npm", "start"]
