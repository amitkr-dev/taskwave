FROM node:22-alpine
WORKDIR /app
COPY apps/worker/package.json apps/worker/package-lock.json* ./
RUN npm ci --production
COPY apps/worker/ .
CMD ["node", "src/worker.js"]