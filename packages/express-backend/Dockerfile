# Use an official Node.js runtime as the base image
FROM node:14

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy the package.json and package-lock.json files to the working directory
COPY package*.json ./

# Install the application dependencies
RUN npm install

# Copy the remaining application files
COPY . .

# Expose the port on which the Express.js app will run
EXPOSE 5000

# Start the Express.js application
CMD ["npm", "start"]
