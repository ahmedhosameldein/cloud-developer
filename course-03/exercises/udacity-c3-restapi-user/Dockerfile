# Set the base image
FROM node:12
# Create app directory
WORKDIR /usr/src/app
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY package*.json ./
# If you are building your code for production
# RUN npm ci --only=production
# To Install all dependencies
RUN npm ci 
# Copy the rest of the app source code  
COPY . .
# Expose the port 
EXPOSE 8080
# Define the command that should be executed to run the app
CMD [ "npm", "run", "dev" ]