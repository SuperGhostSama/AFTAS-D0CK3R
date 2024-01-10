# Use an official Node.js runtime as a parent image
FROM node:16.14.0

# Set the working directory in the container
WORKDIR /app

# Copy the package.json and package-lock.json files into the container at /app
COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy the rest of the application code into the container at /app
COPY . .

# Make port 4200 available to the world outside this container
EXPOSE 4200

# Define the command to run your application
CMD ["npm", "start"]
