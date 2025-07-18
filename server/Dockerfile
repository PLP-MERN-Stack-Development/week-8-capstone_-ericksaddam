FROM node:18-alpine

WORKDIR /usr/src/app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy source code
COPY . .

# Build the app
RUN npm run build

# Expose the port the app runs on
EXPOSE 10000

# Start the application
CMD ["node", "dist/index.js"]
