FROM node:alpine

WORKDIR /app

COPY . /app/

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]

## docker build . -t node_app
## docker run -p 3000:3000 node_app 

