FROM node:14-alpine

# Determines the working directory where all the work is done (This becomes the home directory essentially)
WORKDIR /usr/app

# Copy just the package.json to the container working directory such that npm can be installed
COPY ./package.json ./

RUN npm install

# Copy the rest of the work within the directory such that items changed in the index.js doesn't cause node to install itself again.
COPY ./ ./

CMD ["npm", "start"]