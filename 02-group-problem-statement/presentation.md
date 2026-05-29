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
    font-size: 1.7em;
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

## 1. Bài Toán Cá Nhân - Cao Văn Hảo (2A202600874)

*   **Hảo #1: Hệ thống điểm danh QR lỗi & dễ gian lận (Top 1)**
    *   *Actor:* 500 sinh viên VinUni + Giảng viên.
    *   *Current Workflow:* SV vào lớp $\rightarrow$ mở app điện thoại $\rightarrow$ kết nối wifi trường $\rightarrow$ quét QR code $\rightarrow$ gặp lỗi tương thích iOS < 16, wifi lag, camera mờ $\rightarrow$ phải điền form phụ.
    *   *Bottleneck:* Quét QR code. Dễ bị gian lận bằng cách chụp màn hình QR gửi qua Zalo điểm danh hộ.
    *   *Success Metric:* Giảm thời gian điểm danh từ 18 phút xuống <1 phút. Lỗi quét giảm về 0%.
*   **Hảo #4: Tìm tài liệu môn học bị phân tán (Top 2)**
    *   Tài liệu nằm trên LMS, Drive, Zalo, Email $\rightarrow$ mất 10-15 phút/lần tìm kiếm.
*   **Hảo #7: Ôn thi không hiệu quả (Top 3)**
    *   Đề cương dài 20-30 trang $\rightarrow$ ôn thi lan man không đúng trọng tâm đề thi thực tế.

---

## 2. Bài Toán Cá Nhân - Vũ Tuấn Hoàng (2A202600830)

*   **Hoàng #1: Lượng kiến thức lý thuyết quá lớn (Learning Overwhelm - Top 1)**
    *   *Actor:* Sinh viên ngành Công nghệ / Data.
    *   *Current Workflow:* Đọc slide/giáo trình 50-100 trang thụ động $\rightarrow$ take note vào vở/Notion $\rightarrow$ đọc đề thực hành $\rightarrow$ quên kiến thức, loay hoay tra cứu lại từ đầu.
    *   *Bottleneck:* Đọc thụ động lượng thông tin lớn gây ngợp và mất thời gian (2-3 tiếng).
    *   *Success Metric:* Giảm thời gian tổng hợp lý thuyết môn học dưới 30 phút/chương; làm đúng lab >80%.
*   **Hoàng #5: "Ác mộng" cài đặt và cấu hình môi trường Lab (Top 2)**
    *   Cài đặt thư viện, kết nối dữ liệu $\rightarrow$ mất 2-3 tiếng sửa lỗi cấu hình không kịp làm lab.
*   **Hoàng #2: Tài liệu học tập môn học phân tán rải rác (Top 3)**
    *   Thông báo, tài liệu trôi trên Zalo, LMS, Teams... $\rightarrow$ chìm tin nhắn, dễ sót deadline.

---

## 3. Bài Toán Cá Nhân - Phạm Quang Huy (2A202600586)

*   **Huy #1: Quá tải ticket hoàn tiền đổi trả ngày Sale lớn (Top 1)**
    *   *Actor:* CSKH Agent sàn e-commerce.
    *   *Current Workflow:* Khách gửi khiếu nại hoàn tiền $\rightarrow$ Agent đọc mô tả $\rightarrow$ check lịch sử đơn và quy chế $\rightarrow$ ra quyết định.
    *   *Bottleneck:* Khách thiếu bằng chứng hình ảnh/video; Agent phải tra cứu thủ công qua nhiều tool.
    *   *Success Metric:* Giảm tỷ lệ ticket thiếu bằng chứng; giảm thời gian xử lý (AHT) mỗi ca xuống 50%.
*   **Huy #2: Sàng lọc CV tuyển dụng quy mô lớn (Recruiting ATS - Top 2)**
    *   Recruiter lọc tay hơn 1000 hồ sơ/đợt $\rightarrow$ CV sai định dạng, thiếu kỹ năng $\rightarrow$ kéo dài Time-to-hire.
*   **Huy #3: IT Helpdesk nội bộ quá tải vì các lỗi vặt (Top 3)**
    *   Lỗi lặp lại (Wi-Fi, cài máy in, quên pass) $\rightarrow$ nhân viên báo lỗi chung chung khiến IT mất thời gian hỏi.

---

## 4. Quá Trình Hội Tụ Nhóm (Phase 3)

### Phân nhóm 9 bài toán cá nhân thành 5 Clusters và chấm điểm Shortlist:

| Ứng cử viên bài toán nhóm | Actor | Workflow | Pain evidence | Impact | Thực thi Lab | So sánh RWA | Hiểu domain | Tổng |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **📱 Hệ thống điểm danh (FaceID)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **📂 Tài liệu phân tán (AI Search)** | 5 | 4 | 4 | 4 | 4 | 4 | 4 | **29** |
| **📝 Ôn thi hiệu quả (AI Study)** | 4 | 3 | 4 | 3 | 3 | 3 | 4 | **24** |
| **💼 Quy trình doanh nghiệp (CSKH/ATS)** | 2 | 4 | 4 | 4 | 2 | 4 | 2 | **22** |

> **Quyết định hội tụ:** Nhóm đồng thuận 3/3 chọn **Hệ thống điểm danh FaceID (Hảo #1)** làm bài toán trọng tâm để đi sâu nghiên cứu và phát triển giải pháp AI.

---

## 5. Biện Luận Loại Bỏ Các Đề Xuất Khác (Hoàng & Huy)

*   **Tại sao loại bỏ bài toán của Vũ Tuấn Hoàng (Học tập & cấu hình Lab)?**
    *   *AI Study:* Khó định lượng mức độ "hiểu/nhớ" của SV để đánh giá hiệu quả MVP.
    *   *Lab Setup:* Lỗi môi trường, xung đột thư viện/OS quá dị biệt, không thể thu thập đủ data lỗi để AI bao quát.
*   **Tại sao loại bỏ bài toán của Phạm Quang Huy (Vận hành doanh nghiệp)?**
    *   *CSKH hoàn tiền / Lọc CV ATS / IT Helpdesk:* Đều có ROI cao nhưng **không thể tiếp cận dữ liệu thật** (CV ứng viên thật, data giao dịch e-commerce) do bảo mật doanh nghiệp. Khó kiểm chứng thực tế (R/W/A).
*   **Tại sao FaceID điểm danh là tối ưu nhất?**
    *   *Dữ liệu khả thi:* Tự thu thập mẫu ảnh SV tại lớp dễ dàng.
    *   *Validation trực quan:* Lắp camera chạy thử nghiệm real-time ngay cửa phòng học.
    *   *AI là duy nhất:* Giải quyết triệt để lỗi thiết bị/wifi và chống gian lận điểm danh hộ 100%.

---

## 6. Sơ Đồ Phễu Chọn Lọc Đề Tài

```text
    ┌──────────────────────────────────────────────┐
    │          9 problems từ 3 thành viên          │  INPUT
    │ (Học tập, Lỗi cài Lab, Điểm danh, Doanh nghiệp)│
    └──────────────────────┬───────────────────────┘
                           │
                           ▼
    ┌──────────────────────────────────────────────┐
    │         Phân nhóm thành 5 Clusters           │  CLUSTERING
    │ (Tài liệu, Ôn thi, Điểm danh, Setup Lab, Biz)│
    └──────────────────────┬───────────────────────┘
                           │
                    ┌──────▼──────┐
                    │  Đánh giá   │  EVALUATION (Tần suất, Pain,
                    │  theo tiêu  │  khả năng lấy dữ liệu thật,
                    │  chí thực tế│  độ khả thi triển khai lab)
                    └──────┬──────┘
                           │
              ┌────────────▼────────────┐
              │  Hệ thống điểm danh    │  WINNING CANDIDATE
              │  (Tần suất cao, pain    │
              │  nặng, dễ lấy data SV)  │
              └────────────┬────────────┘
                           │
                    ┌──────▼──────┐
                    │  ★ WINNER ★ │
                    │   FaceID    │  OUTPUT
                    │  Điểm danh  │
                    └─────────────┘
```

---

## 7. Kiểm Chứng Thực Tế Bài Toán Điểm Danh (Validation)

### Nhóm tiến hành thu thập minh chứng và khảo sát nhanh:
*   **Khảo sát 5 SV ngoài nhóm:** SV phản ánh lỗi app QR liên tục (thiết bị iOS cũ không cài được app, camera mờ, nghẽn mạng wifi giờ cao điểm). Trường cho điền Google Form bù nhưng thời gian duyệt mail sửa Excel mất **24 tiếng**.
*   **Ghi nhận lớp học thực tế (Tiết 2 ngày 29/05):**
    Thầy giáo đứng lớp chủ động hỏi ai bị lỗi chưa điểm danh được, ngay lập tức có **hơn 20 SV giơ tay** (con số thực tế có thể lớn hơn vì lúc đó đang giải lao).
*   **Phân tích Log Chuyên Cần kì trước (1500 lượt):**
    *   **25%** SV phải dùng form dự phòng ít nhất 1 lần/kỳ do app lỗi.
    *   **8%** lượt điểm danh bị ghi nhận vắng oan do sự cố mạng/thiết bị.

---

## 8. Nghiên Cứu Giải Pháp & Phân Tích Khoảng Trống (Gap)

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

## 9. Quy Trình Hiện Tại & Điểm Nghẽn (As-Is Workflow)

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

## 10. Quy Trình Tương Lai Đề Xuất (To-Be Workflow)

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

## 11. So Sánh Hiệu Quả Trước vs Sau Triển Khai

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

## 12. Chuẩn Hóa Phát Biểu Bài Toán (Problem Statement v1)

*   **Actor:** 500 sinh viên chia 3 lớp (~170 SV/lớp) + Giảng viên tại VinUni.
*   **Workflow:** SV qua cửa lớp $\rightarrow$ Camera IP tự động quét mặt $\rightarrow$ AI Server so khớp DB $\rightarrow$ ghi log DB $\rightarrow$ Dashboard realtime.
*   **Bottleneck:** SV đeo khẩu trang/thiếu sáng làm AI không nhận dạng được (tỷ lệ nhỏ, chuyển sang GV check thủ công tại chỗ).
*   **Impact:** Tiết kiệm 8-18 phút lãng phí mỗi buổi học. Loại bỏ 100% tỷ lệ lỗi QR (20-30%) và gian lận điểm danh hộ qua Zalo (10-15%).
*   **Success Metric:** Giảm thời gian điểm danh xuống **<1 phút** (↓95%). Tỷ lệ lỗi quét QR giảm từ 30% xuống **0%**.
*   **AI Boundary:** AI chỉ nhận diện khuôn mặt và lưu log vào DB. Giảng viên giữ quyền tối cao để override/chỉnh sửa kết quả (Human-in-the-loop).

---

## 13. Lựa Chọn Giải Pháp AI: AI Workflow

### So sánh mức độ ứng dụng công nghệ:
1.  **Mức Rule-based (Không dùng AI):** Nâng cấp app QR, bổ sung check GPS/IP/MAC. Rủi ro: Vẫn nghẽn wifi khi 500 SV truy cập cùng lúc và lỗi camera điện thoại.
2.  **Mức AI Workflow (LỰA CHỌN CỦA NHÓM):**
    *   *Giải pháp:* Camera capture $\rightarrow$ AI trích xuất vector khuôn mặt $\rightarrow$ so khớp vector DB $\rightarrow$ ghi log.
    *   *Lý do chọn:* Điểm danh là quy trình tuyến tính cố định. Chỉ cần AI ở bước nhận diện/matching. Các nghiệp vụ cảnh báo, tính chuyên cần dùng logic lập trình rule-based là đủ ổn định.
3.  **Mức AI Agent:** AI tự động quan sát hành vi, tự hỏi đáp khi SV vắng. Rủi ro: Cực kỳ phức tạp, chi phí cao, không cần thiết cho MVP.

---

## 14. Chi Tiết Kiến Trúc Hệ Thống FaceID & Stack Công Nghệ

*   **Mô tả kỹ thuật từng thành phần:**
    *   **Camera IP:** Đặt cố định góc cao tại cửa phòng học, kết nối dây LAN (PoE) truyền tín hiệu RTSP stream 1080p @ 30fps về máy chủ.
    *   **AI Server (FastAPI / Python):**
        1. *Face Detection (OpenCV / Dlib HOG):* Trích xuất frame hình ảnh, phát hiện vị trí các vùng khuôn mặt.
        2. *Face Encoding (ResNet-29):* Chuyển đổi ảnh khuôn mặt thành vector 128 chiều đặc trưng đại diện.
        3. *Face Matching (Euclidean Distance / Cosine Similarity):* So sánh khoảng cách vector với database ảnh sinh viên đã đăng ký trước.
    *   **Rule-based Engine:**
        - Nếu khoảng cách Euclidean $< 0.6$ (độ tin cậy $> 95\%$): Ghi nhận có mặt.
        - Nếu khoảng cách Euclidean $0.6 - 0.7$ ($80-95\%$): Cần kiểm chứng chéo.
        - Nếu khoảng cách $> 0.7$: Bỏ qua hoặc đưa vào danh sách GV duyệt tay (Fallback).
    *   **Tech Stack:** Python (FastAPI), OpenCV, PostgreSQL (lưu vector/chuyên cần), React (Dashboard giảng viên).

---

## 15. Quyết Định Đầu Tư (Final Decision)

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
