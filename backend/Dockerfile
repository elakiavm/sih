FROM node:14-alpine AS backend
ENV NODE_ENV backend
WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

# ENV PORT $PORT || 3001

EXPOSE 3001

CMD [ "npm","start" ]