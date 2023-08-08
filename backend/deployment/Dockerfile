FROM node:16.19-alpine


# Add configuration here
WORKDIR /app
COPY package*.json ./
COPY src ./src
COPY .gitignore ./
COPY tsconfig.json ./
COPY README.md ./
RUN npm install
RUN npm run build
EXPOSE 4000
CMD ["node", "build/index.js"]
