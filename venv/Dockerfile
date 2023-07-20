FROM node:1.14-alpine AS builder
# Add a work directory
WORKDIR /app
# cache and install dependencies
COPY package.json .
RUN npm install
# Copy app files
COPY . .
# Expose port 
EXPOSE 3000
# Build the app
RUN npm build
# Run the application
CMD ["npm","start"]
