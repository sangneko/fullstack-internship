# Báo cáo kết quả – Task 02: Employee Management (HTML thuần)

## 1. Những kiến thức HTML mới đã tìm hiểu
- **HTML5 & Semantic HTML:** Hiểu cách sử dụng các thẻ có ngữ nghĩa (`<header>`, `<nav>`, `<main>`, `<section>`, `<footer>`) để cấu trúc trang web rõ ràng thay vì lạm dụng `<div>`.
- **HTML5 Form Validation:** Sử dụng các thuộc tính tích hợp sẵn của trình duyệt như `required`, `type="email"`, `type="tel"`, `type="date"` để kiểm tra dữ liệu đầu vào cơ bản mà chưa cần JavaScript.
- **Cấu trúc bảng chuẩn:** Phân tách rõ phần tiêu đề (`<thead>`) và phần nội dung (`<tbody>`) trong `<table>`.

## 2. Các thẻ HTML đã sử dụng và chức năng
- `<!DOCTYPE html>`, `<html>`, `<head>`, `<meta>`, `<title>`, `<body>`: Khai báo tài liệu HTML5 và cấu trúc khung trang.
- `<header>`, `<h1>`, `<p>`: Phần đầu trang, hiển thị tên hệ thống và mô tả.
- `<nav>`, `<ul>`, `<li>`, `<a>`: Thanh điều hướng gồm Dashboard, Employees, Departments, Reports.
- `<main>`, `<section>`, `<h2>`, `<hr>`: Chia nội dung chính thành 2 khu vực rõ ràng (Form thêm nhân viên và Danh sách nhân viên).
- `<form>`, `<label>`, `<input>`, `<select>`, `<option>`, `<textarea>`, `<button>`: Tạo biểu mẫu nhập liệu với các kiểu `text`, `email`, `tel`, `date`, `radio`, danh sách chọn, ô văn bản nhiều dòng và nút `Submit` / `Reset`.
- `<table>`, `<thead>`, `<tbody>`, `<tr>`, `<th>`, `<td>`: Hiển thị bảng danh sách 5 nhân viên giả lập.
- `<footer>`: Phần chân trang hiển thị thông tin bản quyền.

## 3. Cách tổ chức cấu trúc trang web
Trang web được chia thành 4 phần chính theo thứ tự từ trên xuống dưới:
1. **Header:** Tên hệ thống (`Employee Management`).
2. **Navigation:** Thanh menu điều hướng liên kết đến các mục chức năng.
3. **Main:**
   - Section 1: Form nhập thông tin nhân viên mới.
   - Section 2: Bảng danh sách nhân viên hiện có.
4. **Footer:** Thông tin bản quyền.

## 4. Những khó khăn gặp phải và cách xử lý
- **Khó khăn:** Khi chưa dùng CSS, các trường trong form và bảng hiển thị khá sát nhau, khó nhìn.
  - **Cách xử lý:** Sử dụng thẻ `<br>`, `<div>` để xuống dòng hợp lý cho từng trường nhập liệu và thêm thuộc tính `border="1" cellpadding="6" cellspacing="0"` trên `<table>` để bảng dễ đọc hơn.
- **Khó khăn:** Nhóm nút radio `Gender` có thể chọn nhiều ô cùng lúc nếu đặt sai `name`.
  - **Cách xử lý:** Đặt cùng một giá trị `name="gender"` cho cả 3 nút radio (`Male`, `Female`, `Other`) và gắn `<label for="...">` tương ứng với `id` của từng nút.

## 5. Những kiến thức bản thân chưa hiểu rõ
- Cách gửi dữ liệu từ `<form>` lên server thực tế (`action`, `method="post"`) và xử lý dữ liệu đó bằng JavaScript/Backend.
- Cách trang trí bố cục (layout), căn chỉnh khoảng cách và làm đẹp giao diện bằng CSS (Flexbox/Grid).
