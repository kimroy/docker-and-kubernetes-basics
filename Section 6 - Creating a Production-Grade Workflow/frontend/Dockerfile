# Installs dependencies and creates the build for production env
FROM node:16-alpine as builder
WORKDIR /app
COPY package.json .
RUN npm install
COPY . .
RUN npm run build


# Create the run phase with nginx
FROM nginx
COPY --from=builder /app/build /usr/share/html
