ARG VERSION=latest
FROM node:${VERSION}

# set up working dir
WORKDIR /usr/src/app

# copy package.json and package-lock.json
COPY package*.json ./

# install dependencies
RUN yarn install

# Copy the application code from the source code directory
COPY ../../../../SourceCode/99Tech/ScalechatAPI .

# Expose the port
EXPOSE 3000

# Start the application
CMD ["yarn", "server"]
