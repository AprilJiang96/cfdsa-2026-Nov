FROM node:26

WORKDIR /app

COPY package*.json ./
COPY main.js ./
COPY views ./views
COPY public ./public

RUN npm install

ENV PORT=3000
# Set the application name, will be displayed above the image
ENV INSTANCE_NAME=""
# Set the application hash, will be displayed above the image
ENV INSTANCE_HASH=""

EXPOSE ${PORT}

CMD ["node", "main.js"]