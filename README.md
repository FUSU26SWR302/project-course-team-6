# Digital Job Matching System (DJMS)

## 1. Giới thiệu dự án
Digital Job Matching System (DJMS) là một nền tảng website giúp kết nối giữa **Freelancer** (người làm tự do) và **Nhà tuyển dụng**. 
Dự án tập trung vào các công việc làm online (như thiết kế, viết lách, lập trình). Nhà tuyển dụng đăng dự án, còn Freelancer sẽ vào xem và báo giá để nhận việc.

## 2. Hàm lượng nghiên cứu (RBL)
Dự án này nhóm tập trung nghiên cứu các phần chính sau:

### 2.1 Kiến trúc hệ thống
* **Mô hình MVC:** Cách tổ chức code rõ ràng, dễ quản lý và sửa lỗi.
* **Quy trình Thanh toán tạm giữ (Escrow):** Nghiên cứu cách giữ tiền trung gian để đảm bảo an toàn (Người thuê trả tiền -> Web giữ -> Làm xong -> Freelancer nhận tiền).

### 2.2 Công nghệ tích hợp
* **Thanh toán VNPay:** Cách kết nối với cổng thanh toán VNPay để nạp tiền và thanh toán qua mã QR.
* **AI Chatbot (Gemini):** Cách dùng AI của Google để giúp người dùng tìm việc nhanh bằng cách nhắn tin hỏi đáp tự nhiên.

### 2.3 Thuật toán & Logic
* **AI Matching:** AI sẽ tự động đọc dữ liệu từ database của web để gợi ý đúng công việc mà Freelancer đang cần.
* **Hệ thống Report & Anti-Scam:** Cách nhận diện các từ khóa lừa đảo trong khung chat và cho phép người dùng báo cáo vi phạm.

## 3. Công nghệ sử dụng
* **Giao diện (Frontend):** ReactJS, TailwindCSS.
* **Hệ thống (Backend):** NodeJS / Java.
* **Cơ sở dữ liệu:** SQL Server.
* **Công cụ hỗ trợ:** Gemini AI, VNPay.

## 4. Các tính năng chính
* **Freelancer:** Tạo hồ sơ cá nhân, dùng AI để tìm việc, gửi báo giá (Bidding), nộp sản phẩm và rút tiền.
* **Nhà tuyển dụng:** Đăng tin tuyển dụng, chọn người làm, thanh toán giữ tiền qua VNPay, nghiệm thu và đánh giá.
* **Admin:** Duyệt bài đăng, quản lý người dùng, xử lý các báo cáo vi phạm (Report) và duyệt rút tiền.

## 5. Quản lý dự án (Jira)
Mọi công việc và tiến độ của các thành viên đều được theo dõi tại đây:
🔗 **Link Jira:** [Digital Job Matching System Board](https://nguyenkimanhduy811.atlassian.net/jira/core/projects/DJMS/board?filter=&groupBy=none)

## 6. Cách cài đặt cơ bản
1. Cài đặt database SQL Server bằng file script đi kèm.
2. Cấu hình mã API Key của AI và VNPay trong code.
3. Chạy Server và mở website để sử dụng.
