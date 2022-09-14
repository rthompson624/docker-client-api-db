# Specify a base image
FROM node:14.20.0-alpine3.16

WORKDIR /app

# Install dependencies
COPY package.json .
RUN npm install 
COPY . .

EXPOSE 3001

# Default command
CMD ["npm", "run", "start"]
