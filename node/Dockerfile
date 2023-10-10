FROM node:18
# Create app directory
WORKDIR /usr/src/
# Install app dependencies
# A wildcard is used to ensure both package.json AND package-lock.json are copied
# where available (npm@5+)
COPY /node/package.json /usr/src
COPY node/ /usr/src
RUN cd /usr/src \
ls -lart
RUN npm install
# If you are building your code for production
# RUN npm ci --omit=dev
# Bundle app source
EXPOSE 8080
CMD [ "node", "server.js" ]