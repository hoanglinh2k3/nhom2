# Tổng Quan Cấu Trúc Trang Web DecorHome

Tài liệu này cung cấp cái nhìn tổng quan về cấu trúc HTML của trang web **DecorHome** - Website bán đồ trang trí nội thất hiện đại.

## 1. Tổng quan dự án

- **Tên trang web**: DecorHome
- **Mục đích**: Giới thiệu và bán các sản phẩm trang trí nội thất (tranh, đèn, gối, v.v.).
- **Công nghệ sử dụng**: HTML5, CSS3, JavaScript (Vanilla).

## 2. Cấu trúc tệp tin

- `index.html`: Tệp HTML chính chứa cấu trúc nội dung của trang.
- `style.css`: Tệp CSS chứa các quy tắc định dạng giao diện.
- `script.js`: Tệp JavaScript xử lý các tương tác (menu mobile, cuộn trang, hiệu ứng).

## 3. Chi tiết cấu trúc HTML (`index.html`)

Trang web được chia thành các phần chính sau đây, nằm trong thẻ `<body>`:

### 3.1. Header (`<header class="header">`)
- **Mục đích**: Điều hướng chính của trang.
- **Thành phần**:
  - **Logo**: Liên kết về trang chủ (`.logo`).
  - **Mobile Menu Button**: Nút mở menu trên thiết bị di động (`.mobile-menu-btn`).
  - **Navigation**: Thanh điều hướng (`<nav>`) chứa các liên kết đến các phần: Trang chủ, Danh mục, Sản phẩm, Về chúng tôi, Liên hệ.

### 3.2. Hero Banner (`<section id="hero">`)
- **Mục đích**: Phần giới thiệu nổi bật đầu trang để thu hút người dùng.
- **Thành phần**:
  - **Nội dung**: Tiêu đề lớn ("Biến ngôi nhà thành tổ ấm"), mô tả ngắn và nút kêu gọi hành động ("Mua sắm ngay").
  - **Hình ảnh**: Ảnh minh họa không gian nội thất hiện đại.

### 3.3. Danh mục sản phẩm (`<section id="categories">`)
- **Mục đích**: Phân loại sản phẩm để người dùng dễ tìm kiếm.
- **Thành phần**:
  - Tiêu đề section.
  - Lưới danh mục (`.category-grid`) chứa các thẻ danh mục (Tranh treo tường, Đồ trang trí bàn, Đèn, v.v.) kèm hình ảnh đại diện.

### 3.4. Sản phẩm nổi bật (`<section id="featured">`)
- **Mục đích**: Hiển thị các sản phẩm tiêu biểu hoặc đang khuyến mãi.
- **Thành phần**:
  - Lưới sản phẩm (`.product-grid`) chứa các thẻ sản phẩm (`.product-card`).
  - Mỗi thẻ sản phẩm bao gồm: Hình ảnh, Nhãn (Mới/Giảm giá), Tên sản phẩm, Giá và Nút "Thêm vào giỏ".

### 3.5. Về DecorHome (`<section id="about">`)
- **Mục đích**: Kể câu chuyện thương hiệu và giá trị cốt lõi.
- **Thành phần**:
  - Văn bản giới thiệu về sứ mệnh và cam kết chất lượng.
  - Hình ảnh minh họa câu chuyện thương hiệu.

### 3.6. Đánh giá khách hàng (`<section class="testimonials">`)
- **Mục đích**: Tăng độ tin cậy thông qua lời chứng thực từ khách hàng.
- **Thành phần**:
  - Lưới đánh giá (`.testimonial-grid`) chứa các thẻ đánh giá.
  - Mỗi thẻ gồm: Nội dung nhận xét, thông tin khách hàng (Avatar, Tên, Địa điểm).

### 3.7. Footer (`<footer id="contact">`)
- **Mục đích**: Chân trang chứa thông tin liên hệ và bản quyền.
- **Thành phần**:
  - **Cột thông tin**: Giới thiệu ngắn gọn.
  - **Cột liên hệ**: Địa chỉ, Email, Hotline.
  - **Cột mạng xã hội**: Các liên kết Facebook, Instagram, Pinterest.
  - **Dòng bản quyền**: Copyright 2024.

## 4. Các tính năng tương tác (JavaScript)

Các tính năng được kích hoạt trong `script.js` dựa trên cấu trúc HTML này:
- **Mobile Menu Toggle**: Đóng/mở menu trên màn hình nhỏ.
- **Smooth Scroll**: Cuộn mượt mà khi nhấp vào các liên kết điều hướng.
- **Fade-in Animation**: Hiệu ứng hiện dần nội dung khi cuộn trang (sử dụng `IntersectionObserver` với class `.fade-in-section`).

## 5. Tài nguyên bên ngoài

- **Fonts**: Sử dụng Google Fonts (Nunito và Playfair Display).
- **Icons**: (Hiện tại chưa sử dụng thư viện icon ngoài, icon menu được vẽ bằng CSS).
- **Images**: Sử dụng hình ảnh từ Unsplash và RandomUser.
