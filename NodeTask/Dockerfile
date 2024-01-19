FROM node:12
WORKDIR /app
COPY package.json /app
RUN npm install
COPY . .
ENV PORT 80
EXPOSE $PORT
VOLUME ["/app/feedback"]
CMD ["node","server.js"]