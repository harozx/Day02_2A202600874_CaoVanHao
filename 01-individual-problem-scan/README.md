# 01 — Individual Problem Scan

> **Học viên:** Cao Văn Hảo — 2A202600874  
> **Ngày:** 29/05/2026

---

## Phase 0 · Worked Example (15 phút)

> **Deliverable:** Hiểu một bài mẫu hoàn chỉnh

### Bài mẫu đã đọc

Mở `02-deliverable-example.md` — case **Weekly Report trước và sau AI** của Minh (Junior PM).

### Những điều tôi chú ý khi đọc

- [x] Cá nhân scan rộng (10 problems, vượt mức 5) trước khi hội tụ.
- [x] Top 3 Problem Cards có actor, workflow, bottleneck, metric, non-AI alternative, quick gut.
- [x] Nhóm hội tụ bằng cluster → shortlist → score, không chỉ bỏ phiếu.
- [x] Research giải pháp (có sẵn trên thị trường chưa?) giúp nhóm không nghĩ trong chân không.
- [x] Workflow trước/sau có thời gian mỗi bước, bottleneck, boundary (AI làm gì, người làm gì), fallback.
- [x] PS v0 → v1 khác nhau: v1 có thêm metric + boundary rõ hơn.

### Self-check

- [x] Tôi hiểu nhóm chỉ chọn **candidate problem**, không chọn ngay Problem Statement.
- [x] Tôi hiểu deep-dive gồm validation, research, workflow, metric, PS và AI decision.

---

## Phase 1 · Individual Scan: tìm 5+ problems (25 phút)

> **Deliverable:** 5+ problem candidates từ trải nghiệm thật

### Scan rộng — 8 problems (Đạt mốc nhận điểm thưởng bonus)

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại + Pain từ người khác | Hệ thống điểm danh QR lỗi & dễ gian lận: không tương thích iOS < 16 (thiết bị cũ không tải/chạy được app), wifi lag khi 500 SV dùng cùng lúc, camera mờ quét lỗi, và SV chụp ảnh QR gửi qua Zalo nhờ người khác điểm danh hộ. | 500 SV + GV | 20-30% SV phải điền form phụ, ước tính 10-15% SV gian lận mỗi buổi |
| 2 | Tốn thời gian | Đăng ký môn học bị nghẽn mạng: Cổng thông tin (portal) đăng ký tín chỉ quá tải do hàng ngàn SV truy cập cùng lúc vào giờ G, khiến SV mất 2-3 tiếng để canh slot học. | SV toàn trường | Nhiều bài viết phàn nàn trên confession sau mỗi kỳ đăng ký môn học |
| 3 | Tốn thời gian | Lịch thi/lịch học thay đổi liên tục phòng học/giờ học nhưng chỉ thông báo qua email hoặc Zalo nhóm, khiến SV dễ bỏ lỡ tin nhắn. | SV toàn trường | Mỗi kỳ có 3-5 lần đổi phòng/giờ, nhiều SV đi nhầm phòng học cũ |
| 4 | Lặp lại + AI có thể tốt hơn | Tìm tài liệu môn học phân tán trên 4-5 nền tảng (LMS, Drive, Zalo, email), không biết file nào là bản mới nhất. | SV + GV | Mất 10-15 phút/lần tìm đúng file, liên tục hỏi lại trên nhóm Zalo |
| 5 | Pain từ người khác | Đặt phòng thư viện/phòng tự học nhóm: phải đến tận nơi hoặc gọi điện kiểm tra do không có hệ thống online, dễ mất công đi lại khi hết phòng. | SV cần học nhóm | Mất 15-20 phút đi lại nhưng thường xuyên hết phòng trống |
| 6 | Tốn thời gian | Họp nhóm khó sắp lịch: 4-5 người có thời khóa biểu khác nhau, trao đổi qua Zalo mất rất nhiều thời gian mới chốt được giờ trống chung. | SV làm bài tập lớn | Mất 1-2 ngày nhắn tin qua lại mới chốt được lịch họp |
| 7 | AI có thể tốt hơn | Ôn thi không hiệu quả: đề cương dài 20-30 trang, SV không biết nên ôn tập trung phần nào cho sát đề thi thực tế. | SV trước kỳ thi | SV ôn tràn lan tất cả các phần nhưng không đạt kết quả mong muốn |
| 8 | Lặp lại + Pain từ người khác | Quên mang thẻ sinh viên vật lý: Trường bắt quét thẻ từ vật lý để qua cổng an ninh gửi xe và cửa thư viện/lab. SV hay quên thẻ ở phòng/balo khác, dẫn đến phải quay về lấy hoặc xếp hàng đăng ký giấy thủ công mất thời gian. | SV + bảo vệ/thủ thư | SV quên thẻ trung bình 1-2 lần/tháng, mất 15-20 phút xử lý thủ công gây nghẽn quầy an ninh. |


### Top 3 — lý do chọn

| Rank | Problem | Lăng kính | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|---|
| 1 | Hệ thống điểm danh QR lỗi & dễ gian lận (#1) | Lặp lại + Pain từ người khác | 500 SV gặp mỗi ngày, workflow rõ, metric tốt, impact cao nhất | Trường có chịu đổi hệ thống không? |
| 2 | Tài liệu phân tán (#4) | Lặp lại + AI tốt hơn | Mọi SV đều gặp, AI search có thể giải, workflow rõ | Trường có cho phép gom tất cả lên 1 nền tảng? |
| 3 | Ôn thi không hiệu quả (#7) | AI có thể tốt hơn | SV mất nhiều thời gian ôn sai trọng tâm, AI có thể gợi ý cá nhân hóa | Đề thi có đủ pattern để AI phân tích không? |

---

## Phase 2 · Top 3 Problem Cards (35 phút)

> **Deliverable:** 3 Problem Cards + draft workflow trước/sau

---

### 🃏 Problem Card #1: Hệ thống điểm danh QR lỗi và dễ gian lận

**Problem 1 câu:**  
Mỗi buổi học, 20-30% trong 500 SV không thể quét QR code điểm danh do thiết bị cũ không tải được app (yêu cầu iOS 16+), wifi trường nghẽn khi 500 SV truy cập cùng lúc, và camera mờ quét lỗi — dẫn đến việc phải điền form phụ mất thời gian và tình trạng gian lận quét hộ qua Zalo.

**Actor:** Sinh viên (500 SV chia 3 lớp, mỗi lớp ~170 người)

**Thời điểm / bối cảnh:** Đầu mỗi buổi học, GV bật QR code trên máy chiếu 2-3 phút.

**Current workflow:**

```text
CURRENT STATE — 8-18 phút

[1 SV vào lớp: 0']
→ [2 Mở app trên ĐT: 1']  ← thiết bị cũ không được hỗ trợ (iOS < 16 không tải được)
→ [3 Kết nối wifi trường: 2']  ← 500 SV cùng lúc → nghẽn mạng
→ [4 Chờ GV bật QR: 1']
→ [5 Quét QR code: 2']  ← BOTTLENECK: cam mờ, app lag, QR hết hạn, quét hộ qua Zalo
→ [6 App lỗi hoặc không dùng được → điền form phụ: 3-5']  ← 20-30% SV phải làm
→ [7 GV chờ hoặc gọi tên: 5-10']  ← nếu lỗi kết nối diện rộng
Tổng: 8-18 phút/buổi
```

**Bottleneck:** Bước 5 — quét QR code. Tất cả lỗi tập trung: camera mờ, app lag vì wifi, ĐT không tương thích. 500 SV dùng wifi cùng lúc khiến mạng nghẽn.

**Impact:** 500 SV × mỗi ngày × 8-18 phút = **4.000-9.000 phút lãng phí/ngày** toàn trường. 20-30% SV phải điền form phụ thay vì tập trung học.

**Success metric:** Giảm thời gian điểm danh từ 8-18 phút xuống <1 phút. Giảm tỷ lệ cần form phụ từ 20-30% xuống 0%.

**Non-AI alternative:**
- Fix app QR: vẫn phụ thuộc ĐT + wifi → không giải gốc rễ
- Nâng cấp wifi: tốn kém, vẫn phụ thuộc ĐT
- Gọi tên thủ công: 10 phút/lớp 170 người, không scalable
→ Không giải pháp nào bỏ được ĐT + wifi cùng lúc.

**AI hypothesis:** Camera IP + Face Recognition tự nhận diện SV khi bước vào lớp. Không cần ĐT, không cần wifi (camera nối LAN có dây).

**Quick gut:** **Workflow** — pipeline: capture frame → detect face → recognize → log.

**Fallback:** AI không nhận diện được (đeo khẩu trang, ánh sáng yếu) → SV dùng mã PIN/QR dự phòng trên tablet tại cửa lớp.

### Draft current workflow

```text
CURRENT STATE — 8-18 phút

[1 Vào lớp: 0']
→ [2 Mở app: 1']
→ [3 Wifi: 2']
→ [4 Chờ QR: 1']
→ [5 Quét QR: 2']  <-- BOTTLENECK
→ [6 Form phụ: 3-5']
→ [7 GV chờ: 5-10']
```

### Draft future workflow

```text
FUTURE STATE — <1 phút

[1 SV bước vào lớp: 0']
→ [2 Camera IP nhận diện mặt: 0.5']  ← AI boundary
→ [3 AI match với database: 0.2']  ← AI boundary
→ [4 Ghi log: mã SV + thời gian: 0.1']
→ [5 SV check trên app: tùy chọn]  ← human boundary

Fallback: AI không nhận → SV nhập mã PIN trên tablet cửa lớp.
Boundary: AI chỉ nhận diện + log. GV vẫn quyết định cuối cùng.
```

---

### 🃏 Problem Card #2: Tài liệu môn học phân tán

**Problem 1 câu:**  
SV phải tìm tài liệu môn học trên 4-5 nền tảng khác nhau (LMS, Google Drive, Zalo nhóm, email, website GV), không biết file nào là bản mới nhất — mất 10-15 phút mỗi lần tìm.

**Actor:** Tất cả SV (500 SV) + GV (đăng tài liệu rải rác)

**Thời điểm / bối cảnh:** Trước mỗi buổi học, khi chuẩn bị bài, khi làm bài tập.

**Current workflow:**

```text
CURRENT STATE — 10-15 phút/lần

[1 Cần tài liệu: 0']
→ [2 Check LMS: 3']  ← có thể không có
→ [3 Check Drive: 2']  ← link cũ, không biết folder nào
→ [4 Lướt Zalo nhóm: 3']  ← BOTTLENECK: tin nhắn chìm trong chat
→ [5 Hỏi lại bạn: 2-5']  ← "ê file slide hôm qua đâu?"
→ [6 Tìm được file: 0']
Tổng: 10-15 phút/lần tìm
```

**Bottleneck:** Bước 4 — lướt Zalo nhóm. Tài liệu GV gửi chìm trong hàng trăm tin nhắn, không search được hiệu quả.

**Impact:** 500 SV × 3-4 lần/tuần × 10-15 phút = **15.000-30.000 phút/tuần** lãng phí.

**Success metric:** Giảm thời gian tìm tài liệu từ 10-15 phút xuống <1 phút.

**Non-AI alternative:** GV đăng tất cả lên 1 nền tảng duy nhất (LMS). Nhưng thực tế GV vẫn gửi qua Zalo/email → không kiểm soát được.

**AI hypothesis:** AI indexing + search tất cả nguồn (LMS, Drive, Zalo) → SV hỏi "slide bài 5 môn AI" → AI trả đúng file mới nhất.

**Quick gut:** **Workflow** — collect từ nhiều nguồn → index → search → trả kết quả.

**Fallback:** AI không tìm thấy → hiển thị danh sách tất cả file liên quan để SV tự chọn.

### Draft current workflow

```text
CURRENT — 10-15 phút

[1 Cần file: 0']
→ [2 LMS: 3']
→ [3 Drive: 2']
→ [4 Zalo: 3']  <-- BOTTLENECK
→ [5 Hỏi bạn: 2-5']
```

### Draft future workflow

```text
FUTURE — <1 phút

[1 SV hỏi: "slide bài 5 AI": 0']
→ [2 AI search tất cả nguồn: 0.3']  ← AI boundary
→ [3 Trả file mới nhất + link: 0.2']
→ [4 SV download: 0.5']  ← human boundary

Fallback: AI không chắc → hiện top 5 file liên quan.
```

---

### 🃏 Problem Card #3: Ôn thi không hiệu quả

**Problem 1 câu:**  
SV trước kỳ thi không biết nên ôn phần nào, đề cương dài 20-30 trang, ôn tràn lan mất 2-3 ngày mà vẫn thiếu trọng tâm.

**Actor:** SV trước kỳ thi (500 SV, mỗi kỳ 5-6 môn)

**Thời điểm / bối cảnh:** 1-2 tuần trước kỳ thi giữa kỳ và cuối kỳ.

**Current workflow:**

```text
CURRENT STATE — 2-3 ngày ôn/môn

[1 Nhận đề cương: 0']
→ [2 Đọc đề cương 20-30 trang: 2-3 giờ]
→ [3 Không biết phần nào quan trọng: ?]  ← BOTTLENECK
→ [4 Ôn tràn lan tất cả: 1-2 ngày]
→ [5 Làm đề cũ (nếu có): 3-4 giờ]
→ [6 Đi thi, mới biết ôn sai trọng tâm]
```

**Bottleneck:** Bước 3 — không biết phần nào quan trọng. Đề cương dài nhưng không phân loại mức độ ưu tiên.

**Impact:** 500 SV × 5 môn × 2-3 ngày = hàng nghìn ngày ôn không hiệu quả mỗi kỳ.

**Success metric:** Giảm thời gian ôn từ 2-3 ngày/môn xuống 1 ngày/môn, tăng tỷ lệ đạt từ 70% lên 85%.

**Non-AI alternative:** GV highlight phần quan trọng trong đề cương. Nhưng mỗi GV làm khác nhau, không nhất quán.

**AI hypothesis:** AI phân tích đề cương + đề thi cũ → gợi ý phần ôn ưu tiên, tạo quiz cá nhân hóa theo mức hiểu của SV.

**Quick gut:** **Agent** — AI cá nhân hóa theo mức hiểu từng SV.

**Fallback:** AI gợi ý sai trọng tâm → SV vẫn có đề cương gốc để ôn toàn bộ.

