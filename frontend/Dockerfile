# frontend/Dockerfile
FROM node:16

WORKDIR /app
COPY package.json /app/
RUN npm install --include=dev
# --include=dev は本番では外す
COPY . /app/

# パーミッション問題を防ぐ
RUN chown -R node:node /app
USER node

CMD ["npm", "run", "serve"]