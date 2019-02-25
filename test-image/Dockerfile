FROM node:10-slim
COPY package.json .
RUN yarn install
COPY yarn.lock .
COPY index.js .
ADD config "/config"
ENV NODE_CONFIG_DIR="/config"
CMD ["yarn", "start"]
