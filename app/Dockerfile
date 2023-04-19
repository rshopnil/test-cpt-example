# Use the official Node.js 14 image as the base image
FROM node:14

# Set the working directory to /app
WORKDIR /app

# Copy package.json and package-lock.json to the container
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy all files from the project directory to the container
COPY . .

# Expose port 3000
EXPOSE 3000

# Set the startup command to "npm start"
CMD ["node", "server.js"]
