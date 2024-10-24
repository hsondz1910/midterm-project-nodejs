# Sử dụng image Node.js chính thức từ Docker Hub
FROM node:14

# Tạo thư mục làm việc bên trong container
WORKDIR /app

# Sao chép package.json và package-lock.json vào container
COPY package*.json ./

# Cài đặt các dependencies
RUN npm install

# Sao chép toàn bộ mã nguồn ứng dụng vào container
COPY .. .

# Expose port mà ứng dụng sẽ chạy
EXPOSE 3000

# Lệnh khởi động ứng dụng
CMD ["node", "app.js"]
