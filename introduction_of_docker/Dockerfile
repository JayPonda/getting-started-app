# base image
FROM node:18-alpine

# spacify where our wall code will located
WORKDIR /app

# copy current wall code at this level to app directory
COPY package.json yarn.lock ./

# then install necessary packages 
RUN yarn install --production

# run commad in command line to start server
CMD ["node", "src/index.js"]

# expose post 3000 with real port 3000
EXPOSE 3000

