# Use Node.js
FROM node:20-alpine

# Set working directory
WORKDIR /app

# Copy package.json
COPY package.json ./

# Install dependencies
RUN npm install

# Copy all project files
COPY . .

# Expose Vite port
EXPOSE 5173

# Start React (Vite) app
CMD ["npm", "run", "dev", "--", "--host"]