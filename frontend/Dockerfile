# Use an official Node.js runtime as a parent image
FROM node:18

# Expose port 5173 for Vite's development server
EXPOSE 5173

# Set the working directory in the container
WORKDIR /app

# Copy the current directory contents into the container at /app
COPY . /app

# Ensure the .env file is copied into the container
COPY .env /app/.env

# Install any needed packages
RUN npm install

# Use Vite's dev server for development
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
