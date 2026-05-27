# 📍 Find Place - Trình Tìm Kiếm Địa Điểm Bình Yên & Vui Chơi

Chào mừng bạn đến với **Find Place**! Đây là một trang web được lấy cảm hứng từ giao diện tìm kiếm tối giản của Google, giúp người dùng dễ dàng tìm kiếm và định vị các địa điểm "chill" bình yên hoặc các khu vui chơi giải trí sôi động xung quanh mình.

---

## 🚀 Tính Năng Chính
* 🔍 **Tìm kiếm thông minh:** Gõ từ khóa hoặc tìm theo thẻ (Tag) như `binh-yen`, `vui-choi`.
* 🗺️ **Bản đồ trực quan:** Hiển thị vị trí các địa điểm bằng ghim (Marker) trực tiếp trên bản đồ nền Leaflet/OpenStreetMap.
* 🗄️ **Hệ thống dữ liệu:** Quản lý danh sách địa điểm bài bản bằng Backend (Node.js) và Database (MongoDB).

---

## 🛠️ Công Nghệ Sử Dụng

### Giao diện (Frontend)
* HTML5, CSS3 (Giao diện chuẩn Google, bo góc, tối giản)
* JavaScript (ES6+)
* **Leaflet API:** Thư viện hiển thị bản đồ miễn phí

### Hệ thống (Backend & Database)
* **Node.js & Express:** Xử lý các yêu cầu tìm kiếm (API)
* **MongoDB Atlas:** Lưu trữ thông tin địa điểm và tọa độ (Lat/Lng)

---

## 📂 Cấu Trúc Thư Mục Dự Án

* `frontend/` - Chứa toàn bộ giao diện người dùng (HTML, CSS, JS).
* `backend/` - Chứa bộ não xử lý logic và kết nối database.

---

## 🧑‍💻 Hướng Dẫn Cài Đặt và Chạy Trên Máy Cục Bộ (Local)

### 1. Tải dự án về máy
```bash
git clone [https://github.com/ten-tai-khoan-cua-ban/Find_place.git](https://github.com/ten-tai-khoan-cua-ban/Find_place.git)
cd Find_place