# 03 — Individual Reflection

> **Học viên:** Cao Văn Hảo — 2A202600874  
> **Ngày:** 29/05/2026  
> ⚠️ **AI rule:** Không dùng AI viết thay reflection

---

## Phase 7 · Individual Reflection (15 phút)

> **Deliverable:** Reflection cá nhân về vai trò, cách dùng AI, bài học

### Vai trò của mình trong nhóm hôm nay

Trong buổi làm việc nhóm, mình đóng vai trò **người đề xuất giải pháp chính** — mình là người đưa ra ý tưởng FaceID và thuyết phục nhóm rằng đây là giải pháp bao trùm nhất, giải quyết cả 3 vấn đề (app lỗi, gian lận, wifi lag) cùng lúc.

**Điều mình làm tốt:**
- Phân tích được rằng 3 problems của 3 thành viên có **cùng gốc rễ** → gộp lại 1 giải pháp
- Đề xuất dùng camera LAN có dây thay vì wifi — giải quyết triệt để vấn đề lag
- Trình bày workflow trước/sau rõ ràng để nhóm hiểu tại sao FaceID ưu việt hơn fix app

**Điều mình cần cải thiện:**
- Cần tìm hiểu thêm về privacy/bảo mật dữ liệu khuôn mặt — vấn đề nhạy cảm
- Phần tech stack cần research sâu hơn (face_recognition vs DeepFace vs InsightFace)
- Nên hỏi thêm ý kiến GV về khả năng triển khai thực tế tại trường

### Cách mình dùng AI hôm nay

| Phase | Có dùng AI? | Cách dùng | Lưu ý |
|---|---|---|---|
| Phase 0: Đọc bài mẫu | ❌ Không | Tự đọc và phân tích | |
| Phase 1: Scan problems | ❌ Không | Tự brainstorm từ trải nghiệm điểm danh hàng ngày | Tự scan trước, AI sau |
| Phase 2: Problem Cards | ✅ Có | Dùng AI giúp cấu trúc workflow trước/sau rõ ràng hơn | Tự chọn ý, AI giúp format |
| Phase 3: Group pitch | ❌ Không | Tự pitch (AI rule) | Trình bày bằng hiểu biết bản thân |
| Phase 4: Research | ✅ Có | Dùng AI search giải pháp điểm danh trên thị trường | Kiểm tra lại nguồn |
| Phase 5: Workflow + PS | ✅ Có | Dùng AI giúp viết Problem Statement chặt chẽ hơn | Tự kiểm từng bước |
| Phase 6: Decision | ⚠️ Một phần | Nhóm quyết định, AI hỗ trợ phân tích feasibility | Nhóm tự chốt |
| Phase 7: Reflection | ❌ Không | Tự viết | Không copy AI |

### Học được gì

1. **AI là công cụ hỗ trợ, không phải thay thế tư duy.** Phần quan trọng nhất — chọn problem, pitch FaceID cho nhóm, quyết định Go — đều phải tự làm. AI giỏi ở việc research và cấu trúc, nhưng không thể thay thế trải nghiệm cá nhân mỗi buổi điểm danh.

2. **Khi cả nhóm cùng gặp 1 vấn đề → dễ thống nhất.** Thay vì tranh cãi chọn problem nào, nhóm mình nhận ra 3 problems thực chất cùng gốc rễ → gộp lại và chọn giải pháp bao trùm nhất (FaceID).

3. **Giải pháp tốt phải giải gốc rễ, không phải triệu chứng.** Fix app QR = chữa triệu chứng. Thay hẳn bằng FaceID = giải gốc rễ (bỏ ĐT, bỏ wifi, bỏ QR).

4. **Problem first, not AI first.** Mình bắt đầu bằng trải nghiệm thật (app lỗi mỗi ngày), không phải bằng "muốn làm AI gì". Face Recognition chỉ xuất hiện khi đã hiểu rõ workflow và bottleneck.

### Nếu làm lại, mình sẽ đổi gì?

1. **Tư duy đa dạng hơn ngay từ đầu.** Lúc đầu mình bị cuốn vào chủ đề điểm danh nên 3 problems đầu tiên bị trùng lặp gốc rễ. Dù sau đó đã bổ sung thêm các bài toán khác như nghẽn mạng đăng ký tín chỉ hay lịch học/lịch thi thay đổi để đa dạng hóa danh sách 7 problems, nếu làm lại mình sẽ brainstorm rộng hơn ngay từ đầu để tiết kiệm thời gian chỉnh sửa.

2. **Phỏng vấn GV sớm hơn.** Mình chỉ hỏi SV. Nếu hỏi thêm GV và phòng đào tạo, mình sẽ hiểu rõ hơn constraint triển khai thực tế (ngân sách, privacy policy, quy trình phê duyệt).

3. **Viết fallback kỹ hơn từ đầu.** Ban đầu mình chỉ nghĩ happy path (FaceID hoạt động hoàn hảo). Đến Phase 6 mới nghĩ đến edge case (đeo khẩu trang, ánh sáng yếu). Lần sau sẽ nghĩ fallback từ Phase 2.
