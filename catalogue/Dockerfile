FROM node:20
# create /app and set the directoy to /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
ENV MONGO_URL="mongodb://mongodb:27017/catalogue" \
    MONGO="true"
# ExecStart=/bin/node /app/server.js
CMD ["node", "server.js"]

