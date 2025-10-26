# base image
FROM node:20-alpine

# work dir
WORKDIR /app

#copy package.json
COPY package*.json .

#install dependencies
RUN npm install

#copy remaining files
COPY . .

#expose port
EXPOSE 3001

#execute command
CMD ["node", "index.js"]