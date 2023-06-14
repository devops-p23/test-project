FROM node:14-alpine

# Create a working directory for our app
WORKDIR /app

# Copy over the rest of our app
COPY . /app

# Copy over our package.json and package-lock.json files
# COPY package*.json ./

# Install app dependencies
RUN npm install

# Copy over the rest of our app
COPY . /app

# Build the app
RUN npm run build

# Expose the port that our app will run on
EXPOSE 9000

# Start the app
CMD [ "npm", "start" ]
