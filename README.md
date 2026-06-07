# Hệ thống Công nghệ Bất động sản TH-PropTech

Hệ sinh thái ứng dụng tích hợp công nghệ mô phỏng 3D tương tác, thực tế ảo (VR 360°) và trí tuệ nhân tạo (AI/OCR) nhằm tối ưu hóa công tác giới thiệu dự án và tự động hóa quy trình xác thực thông tin giao dịch bất động sản.

---

## Các phân hệ chính trong hệ thống

Dự án được cấu trúc thành các phân hệ độc lập nhằm phục vụ mục đích phát triển song song và dễ dàng tích hợp:

1. **Phân hệ Bản đồ tương tác 3D (overvew-3d-360vr)**:
   - Cung cấp mô hình không gian trực quan của dự án trên môi trường web.
   - Tích hợp chế độ mô phỏng góc nhìn người đi bộ (Walk Mode) hỗ trợ người dùng di chuyển thực tế xung quanh khuôn viên công trình.

2. **Phân hệ Tham quan thực tế ảo (vr-tour-360-core)**:
   - Cung cấp trải nghiệm hình ảnh toàn cảnh 360 độ (Panorama VR) bên trong các căn hộ mẫu.

3. **Phân hệ Nhận dạng Giấy tờ tùy thân (python/ID_Recognition)**:
   - Ứng dụng các thuật toán thị giác máy tính và nhận dạng ký tự quang học (OCR) để tự động trích xuất thông tin từ CMND/CCCD của khách hàng.
   - Hỗ trợ giải mã mã QR trên thẻ CCCD gắn chip để thu thập thông tin định danh chính xác phục vụ quy trình lập hợp đồng điện tử.

4. **Phân hệ Máy chủ và Giao diện cốt lõi (frontend & backend)**:
   - Xử lý các luồng nghiệp vụ giao dịch, quản lý tài khoản người dùng và quản trị hệ thống cơ sở dữ liệu.

---

## Khung công nghệ áp dụng

- **Giao diện và Đồ họa**: HTML5, CSS3, JavaScript (ES6+), Tailwind CSS, Three.js.
- **Dịch vụ máy chủ**: Spring Boot (Java) / Node.js.
- **Thị giác máy tính và Học sâu**: Python, OpenCV, PaddleOCR / EasyOCR, FastAPI.
