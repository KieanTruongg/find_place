# Sử dụng các lệnh git

## 1. Nhóm lệnh lưu 
* **git add .** : đưa các file có sự thay đổi vào hàng chờ, chưa đẩy 
* **git commit -m "văn_ bản"** : lưu trạng thái hiện tại của code trong local lại, kèm "văn_bản" để mô tả phiên bản đó

---

## 2. Nhóm lệnh kết nối máy tính ( local) với Github 
* **git remote add origin <link>** : kết nối thư mục code máy (local) với kho lưu trữ ( repository) trên Github
* **git push** : tải các commit từ máy ( local) lên kho lưu trữ ( repository) trên Github
* **git pull** : tải code từ Github về và gộp vào thư mục hiện tại ở máy ( = git fetch + git merch) 

---

## 3. Nhóm xử lý xung đột 
* **git merge <tên_nhánh>** : hợp 1 nhánh khác vào nhánh hiện tại tạo ra "merge commit" để nối 2 nhánh lại, giữ nguyên lịch sử 2 nhánh 
* **git rebase <tên_nhánh>** : cũng hợp code giống lệnh merge nhưng thay vì tạo nhánh nối, nó sẽ đem các commit của nhánh hiện tại đặt nối tiếp vào sau đuôi commit của nhánh được gộp, làm lịch sử biến thành một đường thẳng duy nhất.(em chưa hiểu nì lắm)

---

## 4. Lệnh xem lại và quay lại
* **git log** : hiển thị các phiên bản commit
* **git checkout <tên_nhánh_hoặc_mã_commit>** : di chuyển con trỏ head qua 1 nhánh khác hoặc 1 commit cụ thể
* **git reset --hard <mã_commit>** : đưa dự án về commit cụ thể 
