# syntax=docker/dockerfile:1
# From là chuẩn bị môi trường phiên bản kéo về container
# tạo trong workdir
# copy thư mục vào docker
# yarn install cài đặt vào môi trường tối ưu package
FROM node:18-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000