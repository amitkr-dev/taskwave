# apps/api/Dockerfile
FROM node:22-alpine
WORKDIR /app
COPY apps/api/package.json apps/api/package-lock.json* ./
RUN npm ci --omit=dev
COPY apps/api/ .
EXPOSE 3000
CMD ["node", "src/server.js"]