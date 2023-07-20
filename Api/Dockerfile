FROM node:18

# Create app directory
WORKDIR ./

# Install app dependencies
COPY package*.json ./

RUN npm install
# If you are building your code for production
# RUN npm ci --omit=dev

# Bundle app source
COPY . .

EXPOSE 3001
CMD [ "node", "server.js" ]
