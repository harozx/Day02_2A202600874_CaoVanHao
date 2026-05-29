---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #1e2327
color: #f8f9fa
style: |
  section {
    font-family: 'Helvetica Neue', Arial, sans-serif;
    padding: 40px;
  }
  h1 {
    color: #4dabf7;
  }
  h2 {
    color: #3b5bdb;
  }
  footer {
    font-size: 0.5em;
    color: #868e96;
  }
  .highlight {
    color: #ffd43b;
    font-weight: bold;
  }
  .success {
    color: #51cf66;
    font-weight: bold;
  }
  .warning {
    color: #ff6b6b;
    font-weight: bold;
  }
---

# 🤖 HỆ THỐNG ĐIỂM DANH FACEID TỰ ĐỘNG
## Giải Pháp Thay Thế App QR & Chống Gian Lận Học Đường
***
**Nhóm 2A:** Vũ Tuấn Hoàng · Cao Văn Hảo · Phạm Quang Huy
**Ngày:** 29/05/2026

---

## 1. Top 3 Bài Toán Của Các Thành Viên

* **Vũ Tuấn Hoàng (Learning & Lab):**
  - Ngợp lý thuyết môn học chuyên ngành (slide 50-100 trang).
  - Cơn ác mộng cấu hình môi trường chạy Lab / kết nối hệ thống.
  - Thông báo & tài liệu học tập bị rải rác nhiều kênh (Zalo, LMS...).

* **Phạm Quang Huy (Doanh nghiệp):**
  - Quá tải ticket hoàn tiền đổi trả e-commerce dịp Sale lớn.
  - Đọc lọc tay CV số lượng lớn trong chiến dịch tuyển dụng (ATS).
  - IT Helpdesk nội bộ quá tải do các lỗi cơ bản lặp đi lặp lại.

* **Cao Văn Hảo (Điểm danh học đường):**
  - App QR trường bị lỗi tương thích thiết bị, nghẽn wifi và gian lận.

---

## 2. Tại Sao Chọn Giải Pháp Điểm Danh FaceID?

### Biện luận so sánh & lý do hội tụ:
1. **Khả thi về dữ liệu (Data Feasibility):** Dễ dàng chụp ảnh khuôn mặt SV trong lớp (với sự đồng ý) để huấn luyện. Khác với Huy (không thể xin CV thật hay data khách hàng Shopee do bảo mật).
2. **Kiểm chứng thực tế nhanh (Validation):** Lắp đặt camera LAN chạy thử nghiệm ngay cửa lớp học. Khác với Hoàng (lỗi cấu hình Lab/môi trường quá phức tạp và bất quy tắc để AI bao quát).
3. **AI là duy nhất & tối ưu:** Nhận diện khuôn mặt loại bỏ hoàn toàn việc dùng điện thoại cá nhân và wifi trường, đồng thời chống điểm danh hộ 100%.

---

## 3. Quy Trình Hiện Tại (As-Is) vs Tương Lai (To-Be)

* **Hiện tại (8 bước, 8-18 phút):**
  SV vào lớp $\rightarrow$ Mở điện thoại $\rightarrow$ Kết nối wifi trường (nghẽn) $\rightarrow$ Đợi GV bật QR $\rightarrow$ Quét QR (lỗi camera/app) $\rightarrow$ Điền form phụ $\rightarrow$ GV duyệt tay trên Excel.
  *(Điểm nghẽn chính: Quét QR & nghẽn mạng)*

* **Tương lai với FaceID (5 bước, <1 phút):**
  SV bước qua cửa $\rightarrow$ Camera IP chụp hình $\rightarrow$ AI Server so khớp database $\rightarrow$ Ghi log DB $\rightarrow$ Đồng bộ dashboard realtime.
  *(Fallback: AI match <80% $\rightarrow$ GV điểm danh tay)*

---

## 4. So Sánh Hiệu Quả Trực Quan

| Tiêu chí | Trước (App QR) | Sau (FaceID) |
| :--- | :---: | :---: |
| **Tổng thời gian** | 8 - 18 phút | **Dưới 1 phút** (↓95%) |
| **Tỷ lệ lỗi** | 20% - 30% | **~0%** |
| **Tỷ lệ gian lận** | 10% - 15% | **0%** (Không thể quét hộ) |
| **Thiết bị SV** | Bắt buộc (iOS 16+) | **Không cần** |
| **Wifi trường** | Nghẽn khi 500 SV vào | **Không phụ thuộc** (Nối LAN) |

---

## 5. Kiến Trúc Hệ Thống FaceID Đề Xuất

* **Mức độ áp dụng:** **AI Workflow** + Rule-based threshold.
* **Luồng xử lý:**
  1. **Camera IP:** Đặt ở cửa lớp, stream video qua LAN.
  2. **AI Server (Python/FastAPI):** OpenCV detect khuôn mặt $\rightarrow$ face_recognition mã hóa vector $\rightarrow$ So khớp database sinh viên.
  3. **Rule Engine:** 
     - Confidence > 95%: Điểm danh có mặt.
     - Confidence 80-95%: Yêu cầu xác minh lại.
     - Confidence < 80%: Đưa vào danh sách chờ GV override (HITL).
  4. **Output:** Realtime Dashboard cho GV & App SV.

---

## 6. Kế Hoạch Triển Khai MVP & Rollback

* **MVP (Pilot nhỏ nhất):**
  - Chạy thử nghiệm tại 1 phòng thực hành (40 SV).
  - Đăng ký trước 5 góc chụp của 40 SV này.
  - Sử dụng 1 camera IP LAN kết nối PC giảng viên.

* **Rollback Plan (Phương án rút lui):**
  - Nếu tỷ lệ nhận diện sai (False Positive) > 5% trong 2 tuần.
  - Hoặc camera mất kết nối > 3 lần/tuần.
  $\rightarrow$ Quay lại hệ thống QR cũ kết hợp Google Form để tối ưu lại AI.

---

# CẢM ƠN THẦY CÔ VÀ CÁC BẠN ĐÃ LẮNG NGHE!
## Q&A
