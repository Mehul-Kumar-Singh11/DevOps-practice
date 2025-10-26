# base image
FROM node:20-alpine

#set working directory
WORKDIR /app

#copy package json files
COPY package*.json .

# npm install 
RUN npm install

#COPY remaining files
COPY . .

# npm run build
RUN npm run build

#EXPOSE PORTS
EXPOSE 5173 

# command to run application
CMD ["npm", "run", "preview"]