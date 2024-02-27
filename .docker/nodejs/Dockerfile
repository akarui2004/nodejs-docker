ARG VERSION=latest
FROM node:${VERSION}

# set up working dir
WORKDIR /usr/src/app

# Copy the application code from the source code directory
COPY ./source/myapp .

# install dependencies
RUN yarn install

# Expose the port
EXPOSE 3000

# Start the application
CMD ["yarn", "server"]
