FROM node:argon

# Create app directory
RUN mkdir -p /ws/src/dockerNode
WORKDIR /ws/src/dockerNode

# Install app dependencies
COPY package.json /ws/src/dockerNode/
RUN npm install

# Bundle app source
COPY . /ws/src/dockerNode

EXPOSE 8080
CMD [ "npm", "start" ]

