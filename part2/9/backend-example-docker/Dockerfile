FROM node:8
WORKDIR /app
COPY . .
RUN npm install
EXPOSE 8000

ENTRYPOINT ["/usr/local/bin/npm", "run", "start"]
