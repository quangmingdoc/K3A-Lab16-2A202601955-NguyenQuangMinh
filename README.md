# README — Lab Teardown Sản phẩm AI: CANVA

## 1. Giới thiệu bài nộp

Đây là bộ hồ sơ nộp bài cho Lab **"Track 1 - AI Product — Teardown sản phẩm AI"** (VLearn Codelabs), phân tích sản phẩm **Canva** theo đúng quy trình 6 bước của lab: chọn sản phẩm → dựng timeline & revert nguyên lý → tệp user & JTBD → 3 dự đoán → AI log & memo → slide & thuyết trình.

M��c tiêu bài không phải là kể lại lịch sử Canva, mà là luyện **product sense**: nhận ra quyết định sản phẩm nào chạy theo nguyên lý nào, và dùng chính kho kinh nghiệm đó để phán đoán hướng đi tiếp theo.

**Sản phẩm phân tích:** Canva
**Nhóm nghiên cứu:** canvaA
**Thời lượng thực hiện:** 120 phút theo khung lab

### Danh sách thành viên & phân công

| MSSV | Họ tên | Vai trò | Phụ trách trong lab |
|---|---|---|---|
| 2A202601235 | **Lê Văn Huy** | Trưởng nhóm | Step 0 (chọn sản phẩm) + Step 1 — Dựng timeline & revert nguyên lý (§1 memo) |
| 2A202601609 | Nguyễn Minh Hoàng | Thành viên | Step 2 — Tệp user & JTBD (§2 memo) |
| 2A202601428 | Hoàng Văn Thành | Thành viên | Step 3 — Ba dự đoán hướng đi (§3 memo) |
| 2A202601955 | Nguyễn Quang Minh | Thành viên | Step 4 — AI log & hoàn thiện memo (§4 memo, ghép bản cuối) |

> Theo đúng nguyên tắc làm việc nhóm của lab: mỗi thành viên phụ trách sâu 1 phần, nhưng timeline (§1) và tệp user/dự đoán (§2–§3) đều được cả nhóm chấm chéo trước khi chốt vào memo — không ai làm việc của phần mình một cách biệt lập.

---

## 2. Cấu trúc file trong bộ nộp bài

```
├── README.md          ← file này — hướng dẫn đọc bộ hồ sơ
├── memo-canva.md       ← memo phân tích chính, 4 phần theo template lab
└── slides.pdf           ← slide thuyết trình (nhóm tự bổ sung trước khi nộp)
```

> ⚠️ Theo yêu cầu nộp bài của lab, chỉ cần nộp **2 file**: `memo.md` (tên file thực nộp: `memo-canva.md`) và `slides.pdf`. File `README.md` này là tài liệu phụ trợ giúp người chấm/đồng đội định vị nhanh nội dung, không thay thế memo.

---

## 3. Nội dung memo-canva.md — tóm tắt nhanh

| Phần | Nội dung | Điểm tối đa |
|---|---|---|
| §1. Timeline các cập nhật lớn | 6 cột mốc từ 2013–2026, mỗi mốc gồm thời điểm · cập nhật · context · nguyên lý revert, kèm 2 link nguồn (Canva Newsroom + báo chí độc lập) | 30đ |
| §2. Tệp user & JTBD | So sánh early adopters (cá nhân không chuyên) vs tệp hiện tại (knowledge worker/marketing/enterprise), JTBD từng tệp viết theo việc cần làm, switching cost theo 4 forces (Push · Pull · Anxiety · Habit) | 20đ |
| §3. Ba dự đoán hướng đi | 3 dự đoán cho 6–12 tháng tới: mở rộng tính năng (agent), mở rộng segment (verticalize), thay đổi mô hình kiếm tiền (usage-based) — mỗi dự đoán đúng 2 dòng, lập luận trỏ về §1 và §2 | 30đ |
| §4. AI Log | Bảng khai báo minh bạch: 6 hàng, mỗi hàng đều có cột kiểm chứng/phán đoán riêng | 10đ |
| *(Thuyết trình + thảo luận — thực hiện trực tiếp trên lớp)* | Không nằm trong memo | 10đ |

**3 nguyên lý cốt lõi được dùng để revert xuyên suốt memo:**
1. **Wrapper vs Moat** — phân biệt tính năng chỉ là lớp mỏng gọi AI bên ngoài (dễ bị model thế hệ sau hấp thụ) với tính năng có moat thật (workflow, brand data, persistent context riêng của Canva).
2. **Vertical AI / Segment expansion** — đánh giá Canva có đang mã hóa domain expertise theo từng phòng ban (marketing, sales, HR) vào hệ thống hay chỉ chạy đua tính năng AI chung chung.
3. **JTBD & Switching Cost (4 forces)** — nhìn Canva qua lăng kính "user thuê nó để hoàn thành việc gì", không phải qua danh sách tính năng; xác định lực nào (Push/Pull/Anxiety/Habit) đang chi phối quyết định ở lại của user.

---

## 4. Vì sao chọn Canva

Canva thỏa đủ 3 tiêu chí chọn sản phẩm của Step 0:
- ✅ **AI đóng vai trò đủ lớn**: từ Text to Image/Magic Write (2022) đến Canva AI 2.0 chạy trên Canva Design Model riêng, có agentic editing và persistent memory (2026).
- ✅ **Đủ dữ liệu công khai**: Canva Newsroom chính thức, đưa tin độc lập từ Forbes, TechRadar, Business Wire, Voicebot.ai — đủ dựng 6 cột mốc có nguồn kiểm chứng chéo (mỗi mốc 2 nguồn).
- ✅ **Use case & JTBD rõ ràng**: từ "tạo thiết kế đẹp không cần học Photoshop" đến "đi từ brief/data đến nội dung hoàn chỉnh, đúng brand, sẵn sàng publish" — đường dịch chuyển JTBD rất rõ để phân tích.

---

## 5. Tóm tắt phát hiện chính (đọc nhanh cho người chấm bận)

- Canva đi qua 3 thời kỳ rõ rệt: **2013–2021 "Everyone can design" (democratize design) → 2022–2025 "Everyone can create content" (AI + Visual Work Suite) → 2026– "Give us the goal, we help execute the work" (agentic creative platform)**.
- Điểm ngoặt quan trọng nhất về mặt nguyên lý: Canva chuyển từ **wrapper** (gọi AI cho Magic Write, 2022) sang **workflow moat** (Magic Studio, 2023) rồi **agent + proprietary context moat** (Canva AI 2.0, 2026) — moat không nằm ở model AI cụ thể mà ở workflow + brand data + design engine + collaboration tích lũy nhiều năm.
- 3 dự đoán trong memo đều bám vào diễn biến này: (1) Canva AI trở thành agent thực thi trọn workflow, (2) verticalize sâu theo phòng ban (Marketing/Sales/HR), (3) chuyển dần sang pricing theo usage/AI allowance thay vì chỉ theo seat.

---

## 6. Checklist trước khi nộp (theo đúng lab)

- [x] Timeline đủ 6–8 mốc, mỗi mốc là quyết định sản phẩm thật (không phải bản vá), có link nguồn
- [x] Mỗi mốc đã revert về 1 nguyên lý có tên (không dán nhãn đại trà kiểu "để tăng trưởng")
- [x] Tệp user đủ cụ thể — gọi tên được "một người thật"; JTBD viết theo việc cần làm, không theo tính năng
- [x] 3 dự đoán đều có lập luận dẫn ngược về §1–§2, không đứng một mình
- [x] AI log khai đủ, trung thực, có kiểm chứng — không chỉ ghi 1 dòng "dùng ChatGPT"
- [x] Đã điền tên nhóm + thành viên vào đầu `memo-canva.md`
- [ ] Đã chuẩn bị `slides.pdf` và luồng trình bày: timeline → nguyên lý → tệp user → 3 dự đoán
- [ ] Sẵn sàng trả lời câu hỏi phản biện: *"Trong 4 forces, lực nào giữ user Canva mạnh nhất — nếu lực đó biến mất thì sao?"* và *"Dự đoán nào nhóm tự tin nhất, giả định nào nếu sai sẽ làm nó gãy?"*

---

## 7. Ghi chú minh bạch về AI

Bài phân tích này có sử dụng AI (web search) để tìm kiếm và tổng hợp thông tin timeline từ các nguồn công khai (Canva Newsroom, Forbes, TechRadar, Business Wire, Voicebot.ai). Toàn bộ việc **chọn mốc nào đưa vào memo, revert nguyên lý, xác định JTBD, và viết 3 dự đoán là phán đoán của nhóm**, có đối chiếu lại với dữ liệu gốc trước khi đưa vào memo. Chi tiết đầy đủ xem tại §4 AI Log trong `memo-canva.md`.

---

*VLearn Codelabs | Học AI thực chiến qua Lab*