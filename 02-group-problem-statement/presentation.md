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
**Nhóm 2A:** Vũ Tuấn Hoàng (2A202600830) · Cao Văn Hảo (2A202600874) · Phạm Quang Huy (2A202600586)
**Giảng viên hướng dẫn:** AI Product Labs Instructor
**Ngày:** 29/05/2026

---

## 1. Top 3 Bài Toán Cá Nhân - Vũ Tuấn Hoàng (2A202600830)

*   **Hoàng #1: Lượng kiến thức lý thuyết quá lớn (Learning Overwhelm)**
    *   *Actor:* Sinh viên ngành Công nghệ / Data.
    *   *Workflow/Bottleneck:* Đọc slide/giáo trình thụ động 50-100 trang $\rightarrow$ tốn 2-3 tiếng take note cơ học nhưng khi thực hành lại quên sạch và phải Google từ đầu.
    *   *Impact:* Stuck code liên tục, mất gốc lý thuyết, điểm đồ án kém.
*   **Hoàng #5: "Ác mộng" cấu hình môi trường làm Lab (Lab Setup)**
    *   *Workflow/Bottleneck:* Cài đặt thư viện, cấu hình OS, kết nối database cho lab mới $\rightarrow$ mất nguyên buổi học (2-3 tiếng) gỡ lỗi môi trường không kịp làm bài Lab.
*   **Hoàng #2: Tài liệu học tập môn học phân tán**
    *   *Workflow/Bottleneck:* GV gửi link, slide, tài liệu rải rác trên Zalo, LMS, Teams, Drive $\rightarrow$ chìm tin nhắn, mất 15 phút tìm kiếm, dễ bị sót deadline quan trọng.

---

## 2. Top 3 Bài Toán Cá Nhân - Phạm Quang Huy (2A202600586)

*   **Huy #1: Quá tải khiếu nại hoàn tiền ngày Sale (CSKH E-Commerce)**
    *   *Actor:* CSKH Agent sàn e-commerce.
    *   *Workflow/Bottleneck:* Đọc giải trình $\rightarrow$ tra cứu lịch sử đơn $\rightarrow$ duyệt. Tuy nhiên, khách thiếu video/ảnh bằng chứng lỗi, Agent mất thời gian check tay.
    *   *Impact:* Agent bị stress vì quá tải ticket; thời gian xử lý tăng cao; khách hàng đánh giá 1 sao.
*   **Huy #2: Sàng lọc CV quy mô lớn (Recruiting ATS)**
    *   *Actor:* Recruiter quản lý mass recruitment (>1000 hồ sơ/đợt).
    *   *Workflow/Bottleneck:* Đọc CV tay $\rightarrow$ CV sai định dạng, thiếu kinh nghiệm/kỹ năng $\rightarrow$ tốn thời gian lọc thủ công, kéo dài Time-to-hire, dễ bỏ sót ứng viên tốt.
*   **Huy #3: IT Helpdesk nội bộ quá tải ticket vặt**
    *   *Workflow/Bottleneck:* Nhân viên công ty nhắn báo lỗi chung chung (Wi-Fi yếu, cài máy in, quên pass) $\rightarrow$ IT phải chat hỏi han, không có thời gian xử lý sự cố hạ tầng lớn.

---

## 3. Top 3 Bài Toán Cá Nhân - Cao Văn Hảo (2A202600874)

*   **Hảo #1: Lỗi app QR điểm danh trường & gian lận**
    *   *Actor:* 500 sinh viên VinUni + Giảng viên.
    *   *Workflow/Bottleneck:* SV vào lớp $\rightarrow$ mở app $\rightarrow$ nghẽn wifi $\rightarrow$ quét QR lỗi (do camera mờ hoặc iOS cũ < 16 không tải được app). Ngoài ra, SV chụp ảnh QR gửi qua Zalo để nhờ điểm danh hộ từ xa.
    *   *Impact:* 20-30% SV bị lỗi phải điền form phụ, ước tính 10-15% SV điểm danh hộ.
*   **Hảo #4: Tìm tài liệu môn học bị phân tán**
    *   *Workflow/Bottleneck:* Tài liệu nằm rải rác trên 4-5 nền tảng $\rightarrow$ mất 10-15 phút/lần tìm kiếm.
*   **Hảo #7: Ôn thi không hiệu quả**
    *   *Workflow/Bottleneck:* Đề cương dài 20-30 trang $\rightarrow$ ôn thi lan man không đúng trọng tâm đề thi thực tế, tốn 2-3 ngày ôn thi sai phương pháp.

---

## 4. Bảng Chấm Điểm & Phân Nhóm Hội Tụ (Clustering)

### Nhóm gom các bài toán thành 5 Clusters chính và đánh giá trên thang điểm 1-5:

| Ứng cử viên bài toán nhóm | Actor | Workflow | Pain evidence | Impact | Thực thi Lab | So sánh RWA | Hiểu domain | Tổng |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **📱 Hệ thống điểm danh (FaceID)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **📂 Tài liệu phân tán (AI Search)** | 5 | 4 | 4 | 4 | 4 | 4 | 4 | **29** |
| **📝 Ôn thi hiệu quả (AI Study)** | 4 | 3 | 4 | 3 | 3 | 3 | 4 | **24** |
| **💼 Quy trình doanh nghiệp (CSKH/ATS)** | 2 | 4 | 4 | 4 | 2 | 4 | 2 | **22** |

*   *Cluster tài liệu phân tán:* Gom Hảo #4 và Hoàng #2.
*   *Cluster ôn tập:* Gom Hảo #7 và Hoàng #1.
*   *Cluster quy trình doanh nghiệp:* Gom Huy #1, Huy #2, Huy #3.

---

## 5. Biện Luận Loại Bỏ Các Bài Toán Khác (Hoàng & Huy)

*   **Tại sao loại bỏ bài toán của Vũ Tuấn Hoàng (Học tập & Lab)?**
    *   *Learning Overwhelm (Hoàng #1) & AI Study (Hảo #7):* Định nghĩa thế nào là "nhớ lâu" hay "hiểu sâu" rất khó đo lường chính xác bằng các chỉ số kỹ thuật. Thuật toán cá nhân hóa học tập đòi hỏi lượng dữ liệu người dùng khổng lồ để kiểm chứng, không khả thi cho MVP ngắn ngày.
    *   *Cấu hình môi trường Lab (Hoàng #5):* Lỗi cài đặt thư viện/môi trường quá dị biệt, phụ thuộc hệ điều hành/phần cứng. Không thể gom đủ dữ liệu lỗi để huấn luyện AI chính xác.
*   **Tại sao loại bỏ bài toán của Phạm Quang Huy (Doanh nghiệp)?**
    *   *CSKH hoàn tiền (Huy #1), Lọc CV (Huy #2), IT Helpdesk (Huy #3):* Đều là bài toán ROI cao nhưng **không thể tiếp cận dữ liệu thật** (CV ứng viên thật, data giao dịch e-commerce) do bảo mật doanh nghiệp. Việc khảo sát recruiter/CSKH agent thực tế rất khó khăn, nhóm chỉ có thể xây dựng trên giả định lý thuyết.

---

## 6. Biện Luận Lựa Chọn Hệ Thống Điểm Danh FaceID (Hảo #1)

*   **Tính khả thi của dữ liệu vượt trội (Data Feasibility):**
    Nhóm có thể tự chụp ảnh khuôn mặt các bạn sinh viên trong lớp (với sự đồng thuận rõ ràng) để làm bộ dữ liệu huấn luyện thật. Dữ liệu thật, trực quan, dễ dán nhãn.
*   **Khả năng thử nghiệm thực tế ngay lập tức (Real Validation):**
    Dễ dàng lắp 1 camera IP LAN ngay tại cửa phòng học thực tế, chạy so khớp real-time và khảo sát lấy ý kiến phản hồi của giảng viên/SV tại phòng học đó.
*   **Workflow đóng khung, nghiệp vụ rõ ràng:**
    Quy trình tuyến tính đơn giản: SV đi qua cửa $\rightarrow$ capture $\rightarrow$ nhận diện $\rightarrow$ ghi log. Giảng viên đóng vai trò kiểm soát (Human-in-the-loop) để override kết quả nếu AI gặp lỗi nhận diện (đeo khẩu trang, thiếu sáng).
*   **AI là duy nhất & giải quyết triệt để:**
    FaceID là giải pháp duy nhất loại bỏ cả điện thoại của SV và wifi trường (dùng LAN có dây cho camera), đồng thời chống gian lận điểm danh hộ 100%.

---

## 7. Sơ Đồ Phễu Chọn Lọc Đề Tài

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

## 8. Kiểm Chứng Trực Thế (Validation Evidence)

*   **Khảo sát nhanh 5 SV ngoài nhóm:**
    *   *Xác nhận:* SV phản ánh thường xuyên bị lỗi app điểm danh của trường, thiết bị cũ không tương thích hệ điều hành, camera mờ, và nghẽn mạng wifi giờ cao điểm.
    *   *Biện pháp:* GV tạm thời cho sinh viên điền Google Form thủ công. Tuy nhiên, quy trình kiểm soát form và sửa Excel tốn 24 tiếng hành chính.
*   **Ghi nhận lớp học thực tế (Tiết 2 ngày 29/05):**
    *   Thầy giáo đứng lớp chủ động hỏi ai bị lỗi chưa điểm danh được buổi sáng, ngay lập tức có **hơn 20 SV giơ tay** (con số thực tế có thể lớn hơn vì lúc đó giờ nghỉ giải lao một số SV đang ngủ hoặc ở ngoài lớp).
*   **Phân tích Log Chuyên Cần kì trước (1500 lượt):**
    *   25% SV phải dùng form dự phòng ít nhất 1 lần/kỳ; 8% lượt điểm danh bị ghi nhận vắng oan do sự cố ứng dụng.

---

## 9. Phân Tích Khoảng Trống Công Nghệ (Gap Analysis)

### Chưa có giải pháp nào giải quyết đồng thời: Tự động hóa + Không dùng ĐT + Chống gian lận

| Tính năng cần có | QR App trường | Gọi tên thủ công | Vân tay | FACEID (ĐỀ XUẤT) |
| :--- | :---: | :---: | :---: | :---: |
| **Không cần ĐT của SV** | ❌ | ✅ | ✅ | **✅** |
| **Tự động hóa (<1 phút)** | ❌ | ❌ | ❌ | **✅** |
| **Chống gian lận 100%** | ❌ | ✅ | ✅ | **✅** |
| **Không phụ thuộc Wifi** | ❌ | ✅ | ✅ | **✅** (Dùng mạng LAN) |
| **Tránh nghẽn xếp hàng** | ⚠️ | ❌ | ❌ | **✅** (Camera quét góc rộng) |
| **Dashboard GV realtime** | ⚠️ | ❌ | ⚠️ | **✅** |

> *Khoảng trống:* QR App nghẽn wifi và dễ gian lận quét hộ qua Zalo. Gọi tên mất 15 phút của lớp 170 SV. Vân tay gây xếp hàng ùn tắc ở cửa. FaceID là giải pháp duy nhất giải quyết triệt để các hạn chế trên.

---

## 10. Quy Trình Điểm Danh Hiện Tại (As-Is)

```text
CURRENT STATE — 8 bước, mất 8-18 phút đầu giờ đối với lớp sĩ số đông (~170 SV)

┌─────────────┐      ┌─────────────┐      ┌─────────────┐      ┌──────────────────┐
│ Bước 1      │      │ Bước 2      │      │ Bước 3      │      │ Bước 4           │
│ SV vào lớp  │───►  │ Mở app ĐT   │───►  │ Kết nối     │───►  │ Chờ GV bật mã QR │
│             │      │             │      │ wifi trường │      │ trên máy chiếu   │
│ Ai: SV      │      │ Ai: SV      │      │ Ai: SV      │      │ Ai: GV           │
│ ⏱ 0'        │      │ ⏱ 1'        │      │ ⏱ 2'        │      │ ⏱ 1'             │
└─────────────┘      └──────┬──────┘      └─────────────┘      └──────────────────┘
                            │ (iPhone < iOS 16                                    
                            │  không tải được)                                    
                            ▼                                                     
                     ┌─────────────┐                                              
                     │ Bước 5      │◄─────────────────────────────────────────────┘
                     │ Quét QR     │
                     │             │ (Lỗi camera mờ, mạng lag,
                     │ Ai: SV      │  gian lận chụp QR gửi Zalo)
                     │ ⏱ 2' 🔴     │ (BOTTLENECK CHÍNH)
                     └──────┬──────┘
                            │
            ┌───────────────┴───────────────┐
            │ (Lỗi quét: 20-30% SV)         │ (Quét thành công: 70-80% SV)
            ▼                               ▼
     ┌─────────────┐                 ┌─────────────┐
     │ Bước 6      │                 │ Bước 7      │
     │ Điền form   │                 │ Hệ thống    │
     │ phụ         │                 │ ghi nhận    │
     │ Ai: SV      │                 │ Ai: App     │
     │ ⏱ 3-5'      │                 │ ⏱ 0'        │
     └──────┬──────┘                 └─────────────┘
            │
            ▼
     ┌─────────────┐
     │ Bước 8      │
     │ GV check &  │
     │ sửa tay     │
     │ Ai: GV      │
     │ ⏱ 5-10'     │
     └─────────────┘
```

---

## 11. Quy Trình Điểm Danh Đề Xuất (To-Be)

```text
FUTURE STATE — 5 bước, chỉ mất <1 phút, tự động hoàn toàn không dùng ĐT & Wifi

┌──────────────┐      ┌──────────────────┐      ┌──────────────────┐
│ Bước 1       │      │ Bước 2           │      │ Bước 3           │
│ SV bước vào  │───►  │ Camera IP capture│───►  │ AI Server match  │
│ cửa lớp      │      │ frame khuôn mặt  │      │ với database     │
│              │      │                  │      │                  │
│ Ai: SV       │      │ Ai: Camera 🔵    │      │ Ai: Model AI 🔵  │
│ ⏱ 0'         │      │ ⏱ 0.5'           │      │ ⏱ 0.2'           │
└──────────────┘      └──────────────────┘      └───────┬──────────┘
                                                        │
                            ┌───────────────────────────┴───────────────────────────┐
                            │ (Match >95%)                                          │ (Match <80% / Lỗi camera)
                            ▼                                                       ▼
                     ┌──────────────┐                                        ┌──────────────┐
                     │ Bước 4       │                                        │ FALLBACK:    │
                     │ Hệ thống ghi │                                        │ GV điểm danh │
                     │ log có mặt   │                                        │ thủ công 🟢  │
                     │ Ai: Server   │                                        └────────────────┘
                     │ ⏱ 0.1'       │                                        
                     └──────┬───────┘                                        
                            │                                                       
                            ▼                                                       
                     ┌──────────────────────────────────────────────────────────────┐
                     │ Bước 5                                                       │
                     │ Dashboard GV realtime & App SV cập nhật trạng thái           │
                     │ Ai: Dashboard + App 🟢                                       │
                     │ ⏱ 0.1'                                                       │
                     └──────────────────────────────────────────────────────────────┘

                     🔵 = AI Boundary (Chạy tự động trên server)
                     🟢 = Human Boundary / Intervention (Giảng viên giám sát & override)
```

---

## 12. Problem Statement v1 (Bản chuẩn hóa)

| Thành phần | Nội dung chi tiết |
| :--- | :--- |
| **Actor** | 500 sinh viên chia 3 lớp (~170 SV/lớp) + Giảng viên tại VinUni. |
| **Workflow** | SV vào lớp $\rightarrow$ Camera IP tự động quét mặt $\rightarrow$ AI Server so khớp DB $\rightarrow$ Ghi log có mặt $\rightarrow$ Hiển thị dashboard real-time. |
| **Bottleneck** | Khẩu trang/thiếu sáng làm AI không nhận dạng được (tỷ lệ nhỏ, chuyển sang GV check thủ công). |
| **Impact** | Tiết kiệm 8-18 phút lãng phí mỗi buổi học. Loại bỏ 100% tỷ lệ lỗi QR (20-30%) và gian lận điểm danh hộ qua Zalo (10-15%). |
| **Success Metric** | Giảm thời gian điểm danh xuống **<1 phút** (↓95%). Tỷ lệ lỗi quét QR giảm từ 30% xuống **0%**. |
| **AI Boundary** | AI chỉ nhận diện khuôn mặt và lưu log vào DB. Giảng viên giữ quyền tối cao để override/chỉnh sửa kết quả (Human-in-the-loop). |
| **AI Intervention**| Bước so khớp khuôn mặt (Face Matching) tự động sau khi camera capture frame cửa lớp. |
| **Mức chọn** | **AI Workflow** kết hợp Rule-based threshold. |

---

## 13. Lựa Chọn Giải Pháp AI: AI Workflow

### Nhóm phân tích và so sánh 3 mức độ ứng dụng công nghệ:

*   **1. Mức Rule-based (Không dùng AI):**
    *   *Giải pháp:* Nâng cấp app QR, check GPS/địa chỉ IP/MAC wifi để xác định vị trí.
    *   *Rủi ro:* Vẫn phụ thuộc điện thoại sinh viên và wifi nghẽn mạng. Không giải quyết được camera mờ.
*   **2. Mức AI Workflow (LỰA CHỌN CỦA NHÓM):**
    *   *Giải pháp:* Kết hợp camera IP chụp hình $\rightarrow$ model AI (OpenCV + face_recognition) trích xuất đặc trưng $\rightarrow$ so khớp vector $\rightarrow$ ghi nhận database.
    *   *Lý do chọn:* Điểm danh là quy trình tuyến tính, cố định tại cửa lớp. AI hoạt động ở bước phát hiện/so khớp, logic nghiệp vụ chạy rule-based là đủ ổn định và tin cậy.
*   **3. Mức AI Agent (Tự trị):**
    *   *Giải pháp:* AI tự động giám sát học viên trong lớp, tự hỏi đáp nếu nghi ngờ vắng mặt.
    *   *Rủi ro:* Chi phí vận hành rất cao, cấu trúc kỹ thuật phức tạp không cần thiết cho MVP.

---

## 14. Kiến Trúc Hệ Thống FaceID Chi Tiết

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

## 15. Quyết Định Đầu Tư (Go / No-Go)

### Đánh giá các tiêu chí quyết định (Tổng điểm: 87%):
*   *Problem có thật?* **100%** (20+ SV giơ tay lỗi, log chuyên cần xác thực).
*   *AI thực sự cần?* **100%** (Chỉ AI mới nhận dạng không cần ĐT & wifi, chống gian lận).
*   *Tính khả thi dữ liệu?* **80%** (Dễ thu thập bộ ảnh mẫu trực tiếp tại lớp).
*   *Năng lực nhóm?* **70%** (Sử dụng các thư viện mã nguồn mở Python có sẵn).

### QUYẾT ĐỊNH CUỐI CÙNG: 🟢 GO

*   **Kế hoạch chạy thử (MVP):** Thử nghiệm tại 1 phòng thực hành (sĩ số 40 SV). Lấy 5 ảnh mẫu của 40 SV này để đăng ký. Dùng 1 camera IP LAN kết nối trực tiếp PC giảng viên.
*   **Kế hoạch rút lui (Rollback):** Nếu tỷ lệ nhận diện sai (False Positive) > 5% trong 2 tuần chạy thử, hoặc camera lỗi kết nối phần cứng > 3 lần/tuần $\rightarrow$ rollback về hệ thống quét QR code cũ kết hợp điền form thủ công để tối ưu hóa lại thuật toán AI.

---

# CẢM ƠN THẦY CÔ VÀ CÁC BẠN ĐÃ LẮNG NGHE!
## Q&A
