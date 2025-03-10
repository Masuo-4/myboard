FROM node:16

WORKDIR /app
COPY package.json package-lock.json* ./
RUN npm install --include=dev

COPY . .
CMD ["npm", "run", "serve"]
