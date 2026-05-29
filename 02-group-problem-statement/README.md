# 02 — Group Problem Statement

> **Nhóm:** Vũ Tuấn Hoàng (2A202600830) · Cao Văn Hảo (2A202600874) · Phạm Quang Huy (2A202600586)  
> **Ngày:** 29/05/2026

---

## Phase 3 · Group Convergence (30 phút)

> **Deliverable:** 1 candidate problem được nhóm chọn  
> ⚠️ **AI rule:** Không dùng AI để pitch/challenge thay mình

### Bước 1: Chia sẻ Top 3 của các thành viên

**Cao Văn Hảo (2A202600874):**
- **Hảo #1:** App QR điểm danh lỗi: không tương thích iOS < 16, wifi lag 500 SV cùng lúc, camera mờ, và gian lận quét hộ qua Zalo.
- **Hảo #4:** Tìm tài liệu môn học bị phân tán trên 4-5 nền tảng (LMS, Drive, Zalo, email) gây mất thời gian.
- **Hảo #7:** Ôn thi không hiệu quả: đề cương dài 20-30 trang, học lan man không sát đề thực tế.

**Vũ Tuấn Hoàng (2A202600830):**
- **Hoàng #1:** Lượng kiến thức lý thuyết quá lớn, dễ bị ngợp và khó áp dụng thực hành.
- **Hoàng #5:** Khó khăn cấu hình môi trường, cài đặt thư viện và kết nối hệ thống khi làm Lab.
- **Hoàng #2:** Thông báo, tài liệu môn học bị phân tán rải rác ở nhiều kênh (Zalo, LMS...).

**Phạm Quang Huy (2A202600586):**
- **Huy #1:** CSKH hoàn tiền đổi trả bị quá tải ngày Sale lớn trong thương mại điện tử.
- **Huy #2:** Lọc CV tuyển dụng quy mô lớn tốn thời gian đọc thủ công (bài toán ATS).
- **Huy #3:** IT Helpdesk nội bộ quá tải vì các lỗi vặt lặp đi lặp lại.

---

### Bước 2: Phân nhóm các bài toán (Clustering)

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| **📂 Tài liệu / thông tin phân tán** | Hảo #4 (tài liệu phân tán) · Hoàng #2 (tài liệu rải rác) | Gom thông tin môn học, tài liệu học tập từ nhiều kênh rải rác về một mối để dễ tra cứu. |
| **📝 Ôn tập & tiếp thu kiến thức** | Hảo #7 (ôn thi lan man) · Hoàng #1 (ngợp lý thuyết) | Hỗ trợ cá nhân hóa quá trình tự học, ôn thi, và tiếp thu kiến thức lớn cho sinh viên. |
| **📱 Hệ thống điểm danh** | Hảo #1 (app QR lỗi & gian lận) | Điểm danh tự động, chính xác, thay thế app quét QR hiện tại của trường. |
| **⚙️ Cấu hình môi trường** | Hoàng #5 (khó cấu hình lab) | Hướng dẫn hoặc tự động hóa thiết lập môi trường kỹ thuật làm lab. |
| **💼 Quy trình doanh nghiệp** | Huy #1 (CSKH hoàn tiền) · Huy #2 (Lọc CV ATS) · Huy #3 (IT Helpdesk) | Tự động hóa các quy trình chăm sóc khách hàng, tuyển dụng, hỗ trợ IT trong vận hành doanh nghiệp. |

---

### Bước 3: Đánh giá và chấm điểm (Shortlist và score)

Nhóm chấm điểm các bài toán ứng viên chính theo thang điểm 1-5 (5 là tốt nhất):

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---|---|---|---|---|---|---|---|
| **📱 Hệ thống điểm danh (FaceID)** | 5 | 5 | 5 | 5 | 5 | 5 | 5 | **35** |
| **📂 Tài liệu phân tán (AI Search)** | 5 | 4 | 4 | 4 | 4 | 4 | 4 | **29** |
| **📝 Ôn thi hiệu quả (AI Study)** | 4 | 3 | 4 | 3 | 3 | 3 | 4 | **24** |
| **💼 Quy trình doanh nghiệp (CSKH/ATS)** | 2 | 4 | 4 | 4 | 2 | 4 | 2 | **22** |

---

### Bước 4: Sơ đồ phễu chọn lọc bài toán

```text
  ╔══════════════════════════════════════════════════════════════╗
  ║              PHỄU CHỌN LỌC PROBLEM (NHÓM)                  ║
  ╚══════════════════════════════════════════════════════════════╝

       ┌─────────────────────────────────────────────┐
       │  9 problems từ 3 thành viên                 │  INPUT
       │  (Học tập, Lab, Doanh nghiệp, Điểm danh...) │
       └───────────────────┬─────────────────────────┘
                           │
                           ▼
       ┌─────────────────────────────────────────────┐
       │  Phân nhóm thành 5 Clusters chính           │  CLUSTERING
       │  (Tài liệu, Ôn tập, Điểm danh, Lab, Biz)     │
       └───────────────────┬─────────────────────────┘
                           │
                    ┌──────▼──────┐
                    │ Đánh giá    │  EVALUATION
                    │ theo 7 tiêu │  (Tần suất, hậu quả,
                    │ chí thực tế │  AI fit, data, feasibility)
                    └──────┬──────┘
                           │
              ┌────────────▼────────────┐
              │  Ứng viên vượt trội:    │  WINNING CANDIDATE
              │  Hệ thống điểm danh     │
              │  (Tần suất cao, pain    │
              │  nặng, dễ lấy data SV)  │
              └────────────┬────────────┘
                           │
                    ┌──────▼──────┐
                    │ Giải pháp   │  SOLUTION
                    │ bao trùm:   │
                    │ FACEID      │
                    └──────┬──────┘
                           │
                    ┌──────▼──────┐
                    │ ★ WINNER ★  │
                    │ FaceID      │  OUTPUT
                    │ điểm danh   │
                    │ tự động     │
                    └─────────────┘
```

**Quyết định cuối cùng của nhóm:** **Chọn Hệ thống điểm danh (FaceID)** làm bài toán trọng tâm.

**Lý do lựa chọn:**
- **Sự đồng thuận (3/3):** Cả nhóm đều trực tiếp trải nghiệm sự bất tiện của hệ thống QR hiện tại hàng ngày.
- **Impact cực lớn:** Tần suất xảy ra hàng ngày với 500 sinh viên toàn khóa. Vắng học quá 4 buổi (>20% thời lượng) đồng nghĩa với việc mất quyền dự thi, nên lỗi điểm danh gây ảnh hưởng cực kỳ nghiêm trọng đến kết quả học tập.
- **Tính khả thi của dữ liệu:** Dự án điểm danh tại trường cho phép nhóm dễ dàng tiến hành khảo sát, lấy dữ liệu khuôn mặt thực tế (với sự đồng thuận) và kiểm chứng hiệu năng. Ngược lại, các bài toán doanh nghiệp của Huy (CSKH, tuyển dụng) dù có ROI cao nhưng cực kỳ khó tiếp cận dữ liệu khách hàng và quy trình thực tế của doanh nghiệp trong thời gian ngắn làm lab.
- **AI là duy nhất:** Chỉ có Face Recognition (AI) mới có thể tự động hóa 100% quá trình nhận dạng mà không cần sinh viên phải thao tác trên điện thoại hay kết nối wifi.

---

## Phase 4 · Validation + Research (30 phút)

> **Deliverable:** Tìm hiểu kiểm chứng + research giải pháp đã có

### 1. Kiểm chứng thực tế (Quick validation)

Nhóm tiến hành khảo sát nhanh 5 sinh viên ngoài nhóm:

| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản xác nhận/phản bác | Nhóm sửa problem thế nào |
|---|---|---|---|---|
| **Khảo sát nhanh SV** | 5 | SV chưa tải được app của nhà trường để quét điểm danh, bị lỗi phiên bản thiết bị, bị camera mờ, và wifi yếu không quét được. | Đến buổi chiều nhà trường đã đưa ra 1 phương án dự phòng là dùng Google Form để SV tự điền điểm danh bù. | Tập trung vào việc xây dựng FaceID tự động độc lập, không phụ thuộc vào app nhà trường hay Google Form điền tay của SV, giúp SV qua cửa lớp là tự ghi nhận. |
| **Ghi nhận thực tế lớp học (Tiết 2 hôm nay)** | Cả lớp (~170 SV) | Thầy giáo đứng lớp chủ động hỏi xem có ai bị lỗi quét mã buổi sáng chưa điểm danh được, ngay lập tức có **hơn 20 SV giơ tay**. | Con số thực tế bị lỗi có thể còn lớn hơn vì thời điểm đó đang giờ nghỉ giải lao, một số bạn đang ngủ hoặc ở ngoài phòng học. | Khẳng định lỗi quét QR xảy ra quy mô lớn trên diện rộng cùng lúc tại lớp học thực tế chứ không phải lỗi cá biệt. Rất cần thiết tự động hóa hoàn toàn. |
| **Phân tích Log Chuyên Cần kì trước** | 1500 lượt | 25% SV phải dùng form dự phòng ít nhất 1 lần trong kì; 8% lượt điểm danh bị ghi nhận vắng oan do sự cố ứng dụng. | Quy trình hành chính cần 24 giờ để giảng viên kiểm tra mail và sửa điểm danh trên Excel. | Tích hợp trực tiếp API nhận diện vào cơ sở dữ liệu chuyên cần của trường để cập nhật trạng thái realtime, giảm độ trễ phản hồi từ 24h xuống <1 giây. |




> 💡 **Insight sau validation:**
> Pain thật của bài toán không nằm ở giao diện app QR đẹp hay xấu. Pain nằm ở việc **nghẽn mạng wifi diện rộng** khi hàng trăm SV cùng truy cập, **sự bất tiện của thiết bị cá nhân** (camera mờ, phiên bản iOS cũ), và **thời gian lãng phí** của giảng viên khi phải kiểm soát thủ công.

---

### 2. Nghiên cứu giải pháp hiện có (Research giải pháp)

Nhóm tìm hiểu các hướng đi hiện tại trên thị trường để tìm kiếm khoảng trống công nghệ:

| Nguồn / tool / case | Link | Họ giải quyết phần nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **App QR hiện tại** | Nội bộ trường | Sinh viên tự dùng ĐT quét mã QR trên máy chiếu lớp. | Chi phí triển khai phần mềm thấp, tận dụng ĐT của SV. | Lỗi tương thích thiết bị, wifi nghẽn giờ cao điểm, dễ gian lận quét hộ qua Zalo. | QR code phụ thuộc thiết bị cá nhân không đảm bảo độ ổn định và tính trung thực. |
| **Gọi tên thủ công** | Truyền thống | Giảng viên đọc tên từng sinh viên trong danh sách. | Chính xác 100%, không cần kết nối mạng. | Mất 10-18 phút mỗi buổi đối với lớp đông (~170 người). | Cần giải pháp tự động hóa để giải phóng thời gian của GV. |
| **Vân tay (Fingerprint)** | Thương mại | Quét vân tay tại máy gắn ở cửa lớp. | Chính xác cao, không thể điểm danh hộ. | SV phải dừng lại xếp hàng quét từng người, tốc độ nhận diện chậm. | Xếp hàng vật lý vẫn tạo bottleneck lớn tại cửa lớp trước giờ học. |
| **ZKTeco SpeedFace** | [zkteco.com](https://www.zkteco.com) | Thiết bị nhận diện khuôn mặt thương mại độc lập. | Nhận diện cực nhanh (<0.5s), chính xác, tích hợp phần cứng chuyên dụng. | Giá thành đắt đỏ ($500-$800/thiết bị), khó tích hợp và đồng bộ sâu với database sinh viên của trường. | Nhóm nên xây dựng một workflow AI linh hoạt, sử dụng camera IP LAN kết nối với máy chủ AI của trường. |

---

### 3. Phân tích khoảng trống công nghệ (Gap Analysis)

```text
  ╔══════════════════════════════════════════════════════════════╗
  ║                        GAP ANALYSIS                          ║
  ╚══════════════════════════════════════════════════════════════╝

  Tính năng cần         QR App   Gọi tên   Vân tay   FACEID (ĐỀ XUẤT)
  ───────────────────  ────────  ────────  ────────  ────────────────
  Không cần ĐT SV         ❌        ✅        ✅            ✅
  Tự động (<1 phút)       ❌        ❌        ❌            ✅
  Chống gian lận          ❌        ✅        ✅            ✅
  Không phụ thuộc wifi    ❌        ✅        ✅            ✅  (LAN có dây)
  Hoạt động ở lab         ❌        ✅        ⚠️            ✅
  Dashboard GV            ⚠️        ❌        ⚠️            ✅
  ───────────────────  ────────  ────────  ────────  ────────────────

  🎯 GAP: Chưa có hệ thống TỰ ĐỘNG + CHỐNG GIAN LẬN + KHÔNG CẦN SV THAO TÁC
```

> **Khoảng trống:** Hệ thống QR hiện tại phụ thuộc hoàn toàn vào thiết bị cá nhân và wifi trường. Gọi tên thủ công thì quá chậm. Vân tay gây tắc nghẽn. FaceID sử dụng camera IP LAN là giải pháp duy nhất đáp ứng đồng thời: tự động nhận dạng khi bước vào cửa, độ chính xác cao, chống gian lận và loại bỏ hoàn toàn việc sử dụng điện thoại/wifi của sinh viên.

---

## Phase 5 · Workflow + Problem Statement (45 phút)

> **Deliverable:** Workflow trước/sau + Problem Statement v0

### 1. Sơ đồ workflow hiện tại (As-Is)

```text
CURRENT STATE — 8 bước, 8-18 phút
┌─────────────┐      ┌─────────────┐      ┌─────────────┐      ┌──────────────────┐
│ Bước 1      │      │ Bước 2      │      │ Bước 3      │      │ Bước 4           │
│ SV vào lớp  │───►  │ Mở app ĐT   │───►  │ Kết nối     │───►  │ Chờ GV bật mã QR │
│             │      │             │      │ wifi trường │      │ trên máy chiếu   │
│ Ai: SV      │      │ Ai: SV      │      │ Ai: SV      │      │ Ai: GV           │
│ ⏱ 0'        │      │ ⏱ 1'        │      │ ⏱ 2'        │      │ ⏱ 1'             │
│ In: Vào cửa │      │ In: ĐT      │      │ In: Wifi    │      │ In: Projector    │
│ Out: Tại chỗ│      │ Out: Màn app│      │ Out: Online │      │ Out: QR hiển thị │
└─────────────┘      └──────┬──────┘      └─────────────┘      └──────────────────┘
                            │ (iPhone < iOS 16                                    
                            │  không tải được)                                    
                            ▼                                                     
                     ┌─────────────┐                                              
                     │ Bước 5      │◄─────────────────────────────────────────────┘
                     │ Quét QR     │
                     │             │ (Lỗi camera mờ, mạng lag,
                     │ Ai: SV      │  gian lận chụp QR gửi Zalo)
                     │ ⏱ 2' 🔴     │
                     │ In: QR code │
                     │ Out: Quét   │
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
     │ In: Link    │                 │ In: Giao dịch│
     │ Out: Form   │                 │ Out: Có mặt │
     └──────┬──────┘                 └─────────────┘
            │
            ▼
     ┌─────────────┐
     │ Bước 8      │
     │ GV chờ /    │
     │ điểm danh   │
     │ Ai: GV      │
     │ ⏱ 5-10'     │
     │ In: Form phụ│
     │ Out: Sửa Excel
     └─────────────┘

🔴 = Bottleneck   ⏱ Tổng: 8-18 phút/buổi
```

- **Actor:** Sinh viên (người thực hiện quét), Giảng viên (bật QR, sửa thông tin).
- **Bottleneck:** Bước 5 (Quét QR). Tại đây camera điện thoại mờ, mạng nghẽn diện rộng, hoặc QR hết hạn trước khi 170 SV kịp quét xong.
- **Bàn giao:** SV quét QR thành công -> App ghi nhận transaction -> Đưa lên database hệ thống -> Giảng viên kiểm tra báo cáo cuối giờ.

---

### 2. Sơ đồ workflow tương lai (To-Be)

```text
FUTURE STATE — 5 bước, <1 phút
┌──────────────┐      ┌──────────────────┐      ┌──────────────────┐
│ Bước 1       │      │ Bước 2           │      │ Bước 3           │
│ SV bước vào  │───►  │ Camera IP capture│───►  │ AI Server match  │
│ cửa lớp      │      │ frame khuôn mặt  │      │ với database     │
│              │      │                  │      │                  │
│ Ai: SV       │      │ Ai: Camera 🔵    │      │ Ai: Model AI 🔵  │
│ ⏱ 0'         │      │ ⏱ 0.5'           │      │ ⏱ 0.2'           │
│ In: Bước đi  │      │ In: Video stream │      │ In: Face Vector  │
│ Out: Mặt cửa │      │ Out: Face crop   │      │ Out: Match ID    │
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
                     │ In: Match ID │                                        
                     │ Out: Log DB  │                                        
                     └──────┬───────┘                                        
                            │                                                       
                            ▼                                                       
                     ┌──────────────────────────────────────────────────────────────┐
                     │ Bước 5                                                       │
                     │ Dashboard GV realtime & App SV cập nhật trạng thái           │
                     │ Ai: Dashboard + App 🟢                                       │
                     │ ⏱ 0.1'                                                       │
                     │ In: DB Log                                                   │
                     │ Out: Màn hình hiển thị                                       │
                     └──────────────────────────────────────────────────────────────┘

🔵 = AI xử lý    🟢 = Human boundary / intervention   ⏱ Tổng: <1 phút
```

- **Actor:** Camera IP (tự động ghi hình), AI Server (xử lý nhận dạng), Giảng viên (giám sát).
- **AI Boundary:** Các bước 2, 3 và 4 chạy tự động trên server AI (Phát hiện -> So khớp -> Ghi log).
- **Human Boundary:** Sinh viên kiểm tra lại kết quả trên App cá nhân. Giảng viên có quyền cao nhất để chỉnh sửa, ghi nhận thủ công nếu có sự cố.
- **Fallback:** So khớp có độ tin cậy < 80% (do đeo khẩu trang, thiếu sáng) hoặc camera hỏng -> Giảng viên chủ động điểm danh thủ công (gọi tên/form bù).


---

### 3. So sánh hiệu quả trực quan

```text
  ╔══════════════════════════════════════════════════════════════╗
  ║                    SO SÁNH TRỰC QUAN TRƯỚC vs SAU            ║
  ╚══════════════════════════════════════════════════════════════╝

  Thời gian:      TRƯỚC ████████████████████ 18 phút
                  SAU   █                    <1 phút    (↓ 95%)

  Tỷ lệ lỗi:      TRƯỚC ████████████████████ 20-30%
                  SAU   ░                    ~0%        (↓ 100%)

  Gian lận:       TRƯỚC ██████████           10-15%
                  SAU   ░                    0%         (↓ 100%)

  Điện thoại SV:  TRƯỚC ████████████████████ Bắt buộc
                  SAU   ░                    Không cần  (Bỏ hẳn)

  Wifi trường:    TRƯỚC ████████████████████ 500 SV cùng lúc
                  SAU   ░                    Dùng LAN   (Bỏ hẳn)
```

| Metric | Trước (QR App) | Sau kỳ vọng (FaceID) | Ghi chú |
|---|---|---|---|
| **Tổng thời gian** | 8 - 18 phút | Dưới 1 phút | Tiết kiệm thời gian dạy học của GV. |
| **Số bước** | 8 bước | 5 bước | Giảm tối đa phiền hà cho sinh viên. |
| **Bước thủ công** | 8/8 bước | 2/5 bước | Sinh viên chỉ cần đi qua cửa lớp, không cần mở app. |
| **Bottleneck chính** | Quét QR (Bước 5) | AI nhận diện & GV check thủ công (nếu lỗi) | Chuyển từ lỗi diện rộng sang xử lý cá nhân. |
| **Rủi ro mới** | Nghẽn mạng, ĐT không tải được app | Nhận diện sai (False Positive) | Yêu cầu mã hóa dữ liệu và cam kết bảo mật. |


---

### 4. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | 500 sinh viên chia làm 3 lớp (~170 SV/lớp) cùng các giảng viên tại VinUni. |
| **Workflow** | SV vào lớp -> mở app ĐT -> kết nối wifi trường -> quét QR code trên máy chiếu -> app báo lỗi/wifi lag -> điền form phụ -> GV sửa điểm danh thủ công. |
| **Bottleneck** | Bước 5: quét QR code (mạng nghẽn do 500 SV truy cập cùng lúc, camera mờ quét lỗi, ĐT cũ không tương thích iOS 16). |
| **Impact** | Lãng phí 8-18 phút đầu giờ. 20-30% SV phải điền form phụ. 10-15% SV gian lận điểm danh hộ qua ảnh Zalo. SV vắng quá 4 buổi mất quyền thi. |
| **Success Metric** | Giảm thời gian điểm danh từ 18 phút xuống <1 phút. Tỷ lệ lỗi quét QR giảm từ 30% xuống 0%. |
| **Boundary** | AI chỉ phát hiện khuôn mặt và lưu log. GV giữ quyền quyết định cuối cùng và override kết quả. |

---

## Phase 6 · Rule / Workflow / Agent + Decision (25 phút)

> **Deliverable:** PS v1 + Go / Not Yet / No-Go

### 1. Phân loại giải pháp AI

Nhóm phân tích ba mức độ ứng dụng AI để lựa chọn giải pháp tối ưu:

| Mức | Phương án | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Nâng cấp app QR hiện có, bổ sung GPS/Wifi MAC kiểm tra vị trí. | Khi 100% SV có thiết bị hỗ trợ và mạng wifi trường cực khỏe. | Vẫn không giải quyết được lỗi camera mờ và nghẽn mạng do truy cập đồng thời. | Không làm toàn bộ, chỉ dùng làm logic rule-based (Confidence > 95% -> Có mặt). |
| **Workflow** | Camera IP tự capture video -> AI Server (OpenCV + face_recognition) nhận diện -> Ghi log DB -> Update dashboard. | Phù hợp vì workflow điểm danh là tuyến tính, cố định tại cửa lớp, database ảnh SV sẵn có. | Nhận diện sai do thiếu sáng, rò rỉ dữ liệu hình ảnh. | **Chọn** (Là lõi của giải pháp vì quy trình khép kín, tuyến tính và rõ ràng). |
| **Agent** | AI tự động quan sát hành vi của SV trong lớp, tự hỏi đáp nếu nghi ngờ SV vắng, tự cập nhật lịch học. | Khi lớp học động, không có cửa lớp cố định. | Chi phí cao, rủi ro kỹ thuật lớn, không cần thiết cho mục tiêu điểm danh. | Chưa chọn (Quá phức tạp đối với MVP). |

- **Mức chọn:** **Workflow** kết hợp Rule-based threshold.
- **Vì sao:** Quy trình điểm danh học đường là tuyến tính (vào lớp -> ghi nhận). AI chỉ cần hoạt động ở bước phát hiện và so khớp khuôn mặt. Các logic nghiệp vụ như tính điểm chuyên cần hay cảnh báo vắng học sử dụng logic lập trình thông thường (rule-based) là đủ, không cần Agent tự trị.

---

### 2. Sơ đồ kiến trúc hệ thống đề xuất

```text
┌─────────────────────────────────────────────────────────────┐
│                 KIẾN TRÚC HỆ THỐNG FACEID                  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  📷 Camera IP (Đặt tại cửa phòng học):                      │
│  └── Kết nối mạng LAN có dây (không lo nghẽn wifi)          │
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

### 3. Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | 500 sinh viên chia 3 lớp (~170 SV/lớp) + giảng viên tại VinUni. |
| **Workflow** | SV vào lớp -> camera IP tự động quét mặt -> AI Server so khớp database -> ghi log có mặt -> dashboard hiển thị realtime. |
| **Bottleneck** | SV đeo khẩu trang/thiếu sáng khiến AI không nhận dạng được (tỷ lệ nhỏ, chuyển sang GV xác minh/điểm danh thủ công). |
| **Impact** | Tiết kiệm 8-18 phút lãng phí mỗi buổi. Loại bỏ hoàn toàn 20-30% trường hợp lỗi quét QR và 10-15% gian lận. |
| **Success Metric** | Giảm thời gian điểm danh từ 18 phút xuống <1 phút (↓95%). Triệt tiêu 100% lỗi QR và gian lận quét hộ. |
| **Boundary** | AI ghi nhận kết quả và lưu log. Giảng viên giữ quyền quyết định cao nhất (Human-in-the-loop) để override kết quả. |
| **AI intervention point** | Bước so khớp khuôn mặt (Face Matching) tự động sau khi camera capture frame cửa lớp. |
| **Mức chọn** | Workflow kết hợp Rule-based threshold. |
| **Rủi ro & người thật kiểm tra** | Rủi ro: AI nhận diện nhầm người (False Positive) hoặc không nhận dạng được. Người thật kiểm tra: SV tự đối chiếu trạng thái trên App SV, giảng viên kiểm tra chéo sĩ số hiển thị trên dashboard đầu giờ và override nếu có sai sót. |

---

### 4. Quyết định đầu tư (Final decision)

```text
  ╔══════════════════════════════════════════════════════════════╗
  ║                        DECISION MATRIX                       ║
  ╚══════════════════════════════════════════════════════════════╝

   Problem có thật?    [████████████████████] 100%  ✅
   AI thực sự cần?     [████████████████████] 100%  ✅
   Tính khả thi cao?   [████████████████░░░░]  80%  ✅
   Giải pháp độc bản?  [█████████████████░░░]  85%  ✅
   Năng lực nhóm OK?   [██████████████░░░░░░]  70%  ⚠️

   Overall Score:      [██████████████████░░]  87%

        ❌ NO-GO         ⚠️ NOT YET        🟢 GO
   ─────────────|────────────────|──────────────────
        0%     30%             60%        ▲       100%
                                          │
                                       87% ★
```

- **Decision:** **🟢 GO**
- **Pilot nhỏ nhất (MVP):** Thử nghiệm tại 1 phòng thực hành (sĩ số ~40 SV). Sử dụng 1 camera IP LAN kết nối trực tiếp với máy tính giảng viên. Đăng ký trước 5 ảnh góc chụp khác nhau của 40 SV này.
- **Exit / rollback:** Nếu tỷ lệ nhận diện sai (False Positive) > 5% trong 2 tuần đầu chạy thử, hoặc camera gặp lỗi kết nối phần cứng > 3 lần/tuần, nhóm sẽ rollback về hệ thống điểm danh QR cũ kết hợp điền form thủ công để tối ưu hóa lại mô hình AI.
- **Decision rationale:** Vấn đề ảnh hưởng trực tiếp hàng ngày đến 500 SV và GV. Giải pháp khả thi do thư viện OpenCV và face_recognition mã nguồn mở rất phát triển, camera IP LAN dễ lắp đặt, dữ liệu khuôn mặt SV có thể chủ động thu thập qua đợt đăng ký đầu kỳ với sự đồng ý của SV (consent form).

---

> **Nhóm:** Vũ Tuấn Hoàng (2A202600830) · Cao Văn Hảo (2A202600874) · Phạm Quang Huy (2A202600586)  
> **Mã HV:** 2A202600830 / 2A202600874 / 2A202600586
