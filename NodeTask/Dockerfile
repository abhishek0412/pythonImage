FROM node:12
ARG DEFAULT_PORT = 80
WORKDIR /app
COPY package.json /app
RUN npm install
COPY . .
ENV PORT $DEFAULT_PORT
EXPOSE $PORT
VOLUME ["/app/feedback"]
CMD ["node","server.js"]