---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #1a1e21
color: #e9ecef
style: |
  section {
    font-family: 'Inter', 'Helvetica Neue', Arial, sans-serif;
    padding: 30px;
    font-size: 20px;
  }
  h1 {
    color: #4dabf7;
    font-size: 1.8em;
    margin-bottom: 10px;
  }
  h2 {
    color: #ffd43b;
    font-size: 1.3em;
    margin-top: 5px;
    margin-bottom: 10px;
  }
  h3 {
    color: #ffd43b;
    font-size: 1.1em;
  }
  footer {
    font-size: 0.55em;
    color: #adb5bd;
  }
  .grid-2 {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
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
  .info {
    color: #339af0;
    font-weight: bold;
  }
  ul {
    margin-top: 5px;
    margin-bottom: 5px;
  }
  li {
    margin-bottom: 5px;
  }
---

# 🤖 BÁO CÁO PHÁT BIỂU BÀI TOÁN NHÓM
## Đề xuất: Hệ Thống Điểm Danh FaceID Tự Động VinUni
***
### Giải pháp thay thế hệ thống QR Code lỗi, chống gian lận & nghẽn mạng
**Nhóm 2A:** Vũ Tuấn Hoàng · Cao Văn Hảo · Phạm Quang Huy
**Ngày:** 29/05/2026

---

## 1. Tổng Quan Quá Trình Hội Tụ Nhóm (Phase 3)

### Phân nhóm 9 bài toán cá nhân thành 5 Clusters và chấm điểm Shortlist:

| Ứng cử viên bài toán nhóm | Actor | Workflow | Pain evidence | Impact | Thực thi Lab | So sánh RWA | Hiểu domain | Tổng |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **📱 Hệ thống điểm danh (FaceID)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **📂 Tài liệu phân tán (AI Search)** | 5 | 4 | 4 | 4 | 4 | 4 | 4 | **29** |
| **📝 Ôn thi hiệu quả (AI Study)** | 4 | 3 | 4 | 3 | 3 | 3 | 4 | **24** |
| **💼 Quy trình doanh nghiệp (CSKH/ATS)** | 2 | 4 | 4 | 4 | 2 | 4 | 2 | **22** |

> **Quyết định hội tụ:** Nhóm đồng thuận 3/3 chọn **Hệ thống điểm danh FaceID (Hảo #1)** làm bài toán trọng tâm để đi sâu nghiên cứu và phát triển giải pháp AI.

---

## 2. Biện Luận Lựa Chọn Đề Tài Đóng Khung Nhóm

*   **Tại sao loại bỏ bài toán của Hoàng (Học tập & cấu hình Lab)?**
    *   *AI Study:* Khó định lượng mức độ "hiểu/nhớ" của SV để đánh giá hiệu quả MVP.
    *   *Lab Setup:* Lỗi môi trường, xung đột thư viện/OS quá dị biệt, không thể thu thập đủ data lỗi để AI bao quát.
*   **Tại sao loại bỏ bài toán của Huy (Vận hành doanh nghiệp)?**
    *   *CSKH hoàn tiền / Lọc CV ATS / IT Helpdesk:* Đều có ROI cao nhưng **không thể tiếp cận dữ liệu thật** (CV ứng viên thật, data giao dịch e-commerce) do bảo mật doanh nghiệp. Khó kiểm chứng thực tế (R/W/A).
*   **Tại sao FaceID điểm danh là tối ưu nhất?**
    *   *Dữ liệu khả thi:* Tự thu thập mẫu ảnh SV tại lớp dễ dàng.
    *   *Validation trực quan:* Lắp camera chạy thử nghiệm real-time ngay cửa phòng học.
    *   *AI là duy nhất:* Giải quyết triệt để lỗi thiết bị/wifi và chống gian lận điểm danh hộ 100%.

---

## 3. Kiểm Chứng Thực Tế Bài Toán Điểm Danh (Validation)

### Nhóm tiến hành thu thập minh chứng và khảo sát nhanh:
*   **Khảo sát 5 SV ngoài nhóm:** SV phản ánh lỗi app QR liên tục (thiết bị iOS cũ không cài được app, camera mờ, nghẽn mạng wifi giờ cao điểm). Trường cho điền Google Form bù nhưng thời gian duyệt mail sửa Excel mất **24 tiếng**.
*   **Ghi nhận lớp học thực tế (Tiết 2 ngày 29/05):**
    Thầy giáo đứng lớp chủ động hỏi ai bị lỗi chưa điểm danh được, ngay lập tức có **hơn 20 SV giơ tay** (con số thực tế có thể lớn hơn vì lúc đó đang giải lao).
*   **Phân tích Log Chuyên Cần kì trước (1500 lượt):**
    *   **25%** SV phải dùng form dự phòng ít nhất 1 lần/kỳ do app lỗi.
    *   **8%** lượt điểm danh bị ghi nhận vắng oan do sự cố mạng/thiết bị.

---

## 4. Nghiên Cứu Giải Pháp & Phân Tích Khoảng Trống (Gap)

### So sánh giải pháp đề xuất với các giải pháp hiện tại:

| Tính năng | QR App trường | Gọi tên thủ công | Vân tay | FACEID (ĐỀ XUẤT) |
| :--- | :---: | :---: | :---: | :---: |
| **Không dùng ĐT của SV** | ❌ | ✅ | ✅ | **✅** |
| **Tự động hóa (<1 phút)** | ❌ | ❌ | ❌ | **✅** |
| **Chống gian lận 100%** | ❌ | ✅ | ✅ | **✅** |
| **Không phụ thuộc Wifi** | ❌ | ✅ | ✅ | **✅** (Camera nối LAN) |
| **Tránh nghẽn xếp hàng** | ⚠️ | ❌ | ❌ | **✅** (Quét diện rộng) |

> *GAP công nghệ:* Chưa có giải pháp nào đồng thời đảm bảo **Tự động nhanh + Không cần điện thoại/mạng SV + Chống gian lận**. FaceID là giải pháp duy nhất lấp đầy khoảng trống này.

---

## 5. Quy Trình Hiện Tại & Điểm Nghẽn (As-Is Workflow)

*   **Quy trình 8 bước tốn 8-18 phút đầu giờ:**
    SV vào lớp $\rightarrow$ Mở app ĐT $\rightarrow$ Kết nối wifi trường (nghẽn mạng) $\rightarrow$ Chờ GV chiếu QR $\rightarrow$ Quét QR code.
*   **Bottleneck chính (Bước 5):** Quét QR code gặp lỗi kết nối/camera hoặc SV chụp ảnh QR gửi Zalo nhờ điểm danh hộ.
*   **Xử lý lỗi (Bước 6, 8):** SV lỗi quét phải điền Form phụ $\rightarrow$ GV phải check email, đối chiếu và sửa thủ công trên file Excel $\rightarrow$ Mất thêm 5-10 phút của giảng viên cuối giờ.

```text
SV vào lớp ──► Mở app ──► Kết nối Wifi ──► Chờ QR ──► [Quét QR (🔴 Bottleneck)]
                                                        │
         ┌─────────────────── Lỗi quét (20-30%) ────────┴───► Thành công (70%)
         ▼
 Điền form phụ ──► GV check mail & sửa tay Excel (Mất 5-10 phút)
```

---

## 6. Quy Trình Tương Lai Đề Xuất (To-Be Workflow)

*   **Quy trình 5 bước tự động hóa (<1 phút):**
    SV đi qua cửa lớp $\rightarrow$ Camera IP tự động capture $\rightarrow$ AI Server so khớp vector $\rightarrow$ Ghi log DB $\rightarrow$ Đồng bộ hiển thị Dashboard/App.

```text
SV qua cửa ──► Camera capture (🔵 AI) ──► Match DB (🔵 AI) ──► Ghi nhận DB (🔵 AI)
                                                                 │
      ┌────────────────── Realtime Sync ─────────────────────────┴──► Dashboard GV & App SV
      ▼
[FALLBACK 🟢]: Match <80% / Lỗi camera ──► GV điểm danh thủ công tại chỗ
```

*   **AI Boundary:** Tự động phát hiện, trích xuất đặc trưng và so khớp vector.
*   **Human Boundary:** Giảng viên giám sát, giữ quyền tối cao override kết quả chuyên cần. Sinh viên kiểm tra trạng thái trên app cá nhân.

---

## 7. So Sánh Hiệu Quả Trước vs Sau Triển Khai

*   **Thời gian điểm danh:**
    *   *Trước:* ████████████████████ 18 phút
    *   *Sau:*   █ <1 phút (Tiết kiệm thời gian giảng dạy)
*   **Tỷ lệ lỗi quét thiết bị/wifi:**
    *   *Trước:* ████████████████████ 20-30%
    *   *Sau:*   ░ 0% (Loại bỏ điện thoại/wifi SV)
*   **Gian lận điểm danh hộ:**
    *   *Trước:* ████████████ 10-15%
    *   *Sau:*   ░ 0% (Chỉ nhận diện người thật trực tiếp)
*   **Độ trễ xử lý lỗi:**
    *   *Trước:* 24 giờ hành chính (qua form phụ và mail)
    *   *Sau:*   <1 giây (đồng bộ real-time dashboard)

---

## 8. Chuẩn Hóa Phát Biểu Bài Toán (Problem Statement v1)

*   **Actor:** 500 sinh viên chia 3 lớp (~170 SV/lớp) + Giảng viên tại VinUni.
*   **Workflow:** SV qua cửa lớp $\rightarrow$ Camera IP tự động quét mặt $\rightarrow$ AI Server so khớp DB $\rightarrow$ ghi log DB $\rightarrow$ Dashboard realtime.
*   **Bottleneck:** SV đeo khẩu trang/thiếu sáng làm AI không nhận dạng được (tỷ lệ nhỏ, chuyển sang GV check thủ công tại chỗ).
*   **Impact:** Tiết kiệm 8-18 phút lãng phí mỗi buổi học. Loại bỏ 100% tỷ lệ lỗi QR (20-30%) và gian lận điểm danh hộ qua Zalo (10-15%).
*   **Success Metric:** Giảm thời gian điểm danh xuống **<1 phút** (↓95%). Tỷ lệ lỗi quét QR giảm từ 30% xuống **0%**.
*   **AI Boundary:** AI chỉ nhận diện khuôn mặt và lưu log vào DB. Giảng viên giữ quyền tối cao để override/chỉnh sửa kết quả (Human-in-the-loop).

---

## 9. Phân Loại Giải Pháp AI: AI Workflow

### So sánh mức độ ứng dụng công nghệ:
1.  **Mức Rule-based (Không dùng AI):** Nâng cấp app QR, bổ sung check GPS/IP/MAC. Rủi ro: Vẫn nghẽn wifi khi 500 SV truy cập cùng lúc và lỗi camera điện thoại.
2.  **Mức AI Workflow (LỰA CHỌN CỦA NHÓM):**
    *   *Giải pháp:* Camera capture $\rightarrow$ AI trích xuất vector khuôn mặt $\rightarrow$ so khớp vector DB $\rightarrow$ ghi log.
    *   *Lý do chọn:* Điểm danh là quy trình tuyến tính cố định. Chỉ cần AI ở bước nhận diện/matching. Các nghiệp vụ cảnh báo, tính chuyên cần dùng logic lập trình rule-based là đủ ổn định.
3.  **Mức AI Agent:** AI tự động quan sát hành vi, tự hỏi đáp khi SV vắng. Rủi ro: Cực kỳ phức tạp, chi phí cao, không cần thiết cho MVP.

---

## 10. Kiến Trúc Hệ Thống FaceID Đề Xuất

```text
    ┌─────────────────────────────────────────────────────────────┐
    │                 KIẾN TRÚC HỆ THỐNG FACEID                  │
    ├─────────────────────────────────────────────────────────────┤
    │                                                             │
    │  📷 Camera IP (Đặt tại cửa phòng học):                      │
    │  └── Kết nối mạng LAN có dây (Tránh nghẽn wifi)             │
    │           │                                                 │
    │           ▼                                                 │
    │  🤖 AI Server (Xử lý nhận diện):                            │
    │  ├── Face Detection: Phát hiện gương mặt (OpenCV)           │
    │  ├── Face Encoding: Mã hóa vector (face_recognition)        │
    │  └── Face Matching: So khớp vector với Database             │
    │           │                                                 │
    │           ▼                                                 │
    │  📋 Rule-based Engine (Phân loại & Xử lý logic):            │
    │  ├── IF match > 95% ──► Điểm danh CÓ MẶT thành công         │
    │  ├── IF match 80-95% ──► Gửi yêu cầu xác minh lại           │
    │  └── IF match < 80% ──► Cảnh báo / Chờ fallback             │
    │           │                                                 │
    │           ▼                                                 │
    │  🔔 Outputs & Dashboard:                                    │
    │  ├── Dashboard Giảng viên: Theo dõi realtime, override      │
    │  ├── App Sinh viên: Tra cứu kết quả điểm danh               │
    │  └── Export báo cáo: File Excel/CSV gửi phòng đào tạo       │
    │                                                             │
    │  💻 Tech Stack: Python (FastAPI) + OpenCV + React + Postgres│
    └─────────────────────────────────────────────────────────────┘
```

---

## 11. Quyết Định Đầu Tư (Final Decision)

### Đánh giá các tiêu chí quyết định (Tổng điểm: 87%):
*   *Problem có thật?* **100%** (Hơn 20 SV giơ tay lỗi, log chuyên cần xác thực).
*   *AI thực sự cần?* **100%** (Chỉ AI mới nhận dạng không cần ĐT & wifi, chống gian lận).
*   *Tính khả thi dữ liệu?* **80%** (Dễ thu thập bộ ảnh mẫu trực tiếp tại lớp).
*   *Năng lực nhóm?* **70%** (Sử dụng thư viện Python có sẵn OpenCV/face_recognition).

### QUYẾT ĐỊNH CUỐI CÙNG: 🟢 GO

*   **Kế hoạch chạy thử (MVP):** Thử nghiệm tại 1 phòng thực hành (40 SV). Lấy 5 ảnh mẫu của 40 SV để đăng ký. Dùng 1 camera IP LAN kết nối trực tiếp PC giảng viên.
*   **Kế hoạch rút lui (Rollback):** Nếu tỷ lệ nhận diện sai (False Positive) > 5% trong 2 tuần chạy thử, hoặc camera lỗi kết nối phần cứng > 3 lần/tuần $\rightarrow$ rollback về hệ thống quét QR code cũ để tối ưu hóa lại thuật toán AI.

---

# CẢM ƠN THẦY CÔ VÀ CÁC BẠN ĐÃ LẮNG NGHE!
## Q&A
