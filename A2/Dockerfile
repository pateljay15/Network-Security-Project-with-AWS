FROM node:latest

# Use production node environment by default.
ENV NODE_ENV production

WORKDIR /app

COPY package*.json ./

RUN npm install

# Run the application as a non-root user.
USER node

# Copy the rest of the source files into the image.
COPY . .

# Expose the port that the application listens on.
EXPOSE 6000

# Run the application.
CMD node index.js
