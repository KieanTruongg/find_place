# Sử dụng các lệnh git

## 1. Nhóm lệnh lưu 
* **git add .** : Đưa các file có sự thay đổi vào hàng chờ, chưa đẩy .
* **git commit -m "văn_ bản"** : Lưu trạng thái hiện tại của code trong local lại, kèm "văn_bản" để mô tả phiên bản đó.
![Sơ đồ khu vực hoạt động của Git](https://raw.githubusercontent.com/jethroconrad/git-workflow-diagram/master/git-workflow-diagram.png)
---

## 2. Nhóm lệnh kết nối máy tính ( local) với Github 
* **git remote add origin <link>** : kết nối thư mục code máy (local) với kho lưu trữ ( repository) trên Github.
* **git push** : Tải các commit từ máy ( local) lên kho lưu trữ ( repository) trên Github.
* **git fetch** : Tải các commit từ kho lưu trữ ( repository) trên Github về máy ( local).
* **git pull** : Tải code từ Github về và gộp vào thư mục hiện tại ở máy ( = git fetch + git merch).

---

## 3. Nhóm xử lý xung đột 
* **git merge <tên_nhánh>** : Hợp 1 nhánh khác vào nhánh hiện tại tạo ra "merge commit" để nối 2 nhánh lại, giữ nguyên lịch sử 2 nhánh 
* **git rebase <tên_nhánh>** : Cũng hợp code giống lệnh merge nhưng thay vì tạo nhánh nối, nó sẽ đem các commit của nhánh hiện tại đặt nối tiếp vào sau đuôi commit của nhánh được gộp, làm lịch sử biến thành một đường thẳng duy nhất.(em chưa hiểu nì lắm)

---

## 4. Lệnh xem lại và quay lại
* **git log** : Hiển thị danh sách lịch sử tất cả các phiên bản commit của nhánh hiện tại (bao gồm mã commit, tác giả, ngày tháng và tin nhắn mô tả).
* **restore** : Huỷ các thay đổi chưa commit, đưa về trạng thái commit gần nhất.
* **git checkout <tên_nhánh_hoặc_mã_commit>** : Di chuyển con trỏ HEAD để chuyển sang một nhánh khác, hoặc quay về xem lại code tại một vị trí commit cụ thể trong quá khứ.
* **git reset --hard <mã_commit>** : Đưa toàn bộ dự án quay về đúng trạng thái của mã commit được chỉ định(lưu ý : toàn bộ các commit nằm sau mốc đó và các đoạn code đang viết dở chưa lưu sẽ bị xóa bỏ hoàn toàn.)
