FROM node:lts-alpine3.18

WORKDIR /usr/src/app

COPY package.json /app

COPY . .

RUN npm set progress=false && npm install

ENV VITE_HOST=0.0.0.0
ENV VITE_PORT=5173

EXPOSE 5173

CMD ["npm", "run","dev"]