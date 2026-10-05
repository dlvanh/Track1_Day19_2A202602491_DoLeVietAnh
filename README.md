# BÀI NỘP TRACK 1 — DAY 19: PROTOTYPING & USER TESTING
## DỰ ÁN VLEARN AI TUTOR: DIAGNOSTIC REFRESHER

> **Khóa học:** AI20K Bootcamp — Cohort 4  
> **Học phần:** Track 1: AI Product Labs (AI Product Design & Prototyping)  
> **Học viên thực hiện:** **Đỗ Lê Việt Anh**  
> **Mã số sinh viên (MSSV):** **2A202602491**  
> **Phương án phụ trách chính:** **Option B** (Chẩn đoán 3 câu — Diagnostic Micro-Check & Knowledge Gap Triage)  
> **Nhóm thực hiện:** **Tung Tung Tung Sahur**  
> **Thành viên nhóm:**  
> - **Lại Bá Quân** (2A202602495) — Lead Option A: *Chỉ vào chỗ kẹt (Inline Term/Block Inspector)*  
> - **Đỗ Lê Việt Anh** (2A202602491) — Lead Option B: *Chẩn đoán 3 câu (3-Question Diagnostic Micro-Quiz)*  
> - **Nguyễn Thị Minh Khánh** (2A202602546) — Lead Option C: *AI gợi ý chủ động (Proactive Context Nudge Card)*  
> - **Nguyễn Quang Huy** (2A202602421) — Lead Option D: *Hỏi người thật (Human Escalation & Auto Context Docket)*  
> **Đơn vị thí điểm:** Nền tảng học tập trực tuyến VLearn  
> **Ngày hoàn thành bài nộp:** 05/10/2026

---

## 📂 Danh Mục 5 Hồ Sơ Bàn Giao (Deliverables Structure)

```
Track1_Day19_2A202602491_DoLeVietAnh/
├── three-option-design-sheet.md       # Bảng phân tích 4 phương án thiết kế A/B/C/D, Human-AI matrix & Next change
├── prototype-link.md                  # Danh sách liên kết nguyên mẫu tương tác A/B/C/D chung của nhóm
├── prototype-feedback-note.md         # Biên bản chi tiết phiên kiểm thử thực tế do chính Việt Anh điều phối (Tester Thiều Quang Vinh)
├── group-feedback-synthesis.md        # Báo cáo tổng hợp phản hồi toàn nhóm & quyết định Next Change thống nhất
├── ai-support-log.md                  # Nhật ký minh bạch sử dụng AI & phản biện của con người
└── prototype/
    └── index.html                     # Mã nguồn nguyên mẫu web tương tác độc lập (Vanilla HTML/CSS/JS)
```

---

## 📌 Tóm Tắt Nội Dung Từng Tài Liệu

### 1. [three-option-design-sheet.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/three-option-design-sheet.md)
- Phân tích chi tiết 4 hướng tiếp cận thiết kế giải quyết điểm nghẽn kiến thức trên nền tảng VLearn:
  - **Phương án A:** *Chỉ vào chỗ kẹt* (Inline Term/Block Inspector - Don't Act) — Quân lead.
  - **Phương án B:** *Chẩn đoán 3 câu* (3-Question Diagnostic Micro-Quiz - Ask) — **Việt Anh lead**.
  - **Phương án C:** *AI gợi ý chủ động* (Proactive Context Nudge Card - Act) — Minh Khánh lead.
  - **Phương án D:** *Hỏi người thật* (Human Escalation & Auto Context Docket - Suggest) — Quang Huy lead.
- 70% Shared Core: 3 Content Fixtures (`context`, `react`, `gd`) áp dụng trên cả Slide lý thuyết và bài thực hành Lab.
- Bảng quyết định Human–AI (Role & Agency, Expectation, Evidence & Uncertainty, Control & Recovery).
- Tổng hợp kết quả User Testing từ 4 phiên và quyết định Next Change tích hợp của nhóm.

### 2. [prototype-link.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype-link.md)
- Tổng hợp toàn bộ liên kết trải nghiệm trực tiếp nguyên mẫu web [`prototype/index.html`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype/index.html).
- Hướng dẫn truy cập nhanh cả 4 options trên 3 kịch bản:
  - Chủ đề 1: Context Window (Slide 12 & Lab 4).
  - Chủ đề 2: ReAct Agent (Slide 9 & Lab 3).
  - Chủ đề 3: Gradient Descent (Slide 7 & Lab 9).
- Bàn điều khiển Facilitator Log (`#/log`) ghi nhận telemetry thời gian thực dạng CSV.

### 3. [prototype-feedback-note.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype-feedback-note.md)
- Biên bản ghi chép phiên kiểm thử định tính 1-1 do chính **Đỗ Lê Việt Anh** trực tiếp điều phối.
- Người tham gia: Bạn **Thiều Quang Vinh** (MHV: **2A202602877**, Học viên AI Thực Chiến khóa 4).
- Thời gian & địa điểm: **13:00 – 13:15 ngày 05/10/2026 trực tiếp tại phòng học 201**.
- Trình tự trải nghiệm: Option A ➔ Option C ➔ Option D ➔ Option C (retest).
- Nhật ký CSV 37 dòng trích xuất từ Facilitator Log ghi nhận chính xác từng giây hành vi làm đúng trước, cố tình làm sai sau để đánh giá AI.
- Phân tích 4 lớp dữ liệu (Observed, Interpreted, Decided - Next Change, Still Unproven).

### 4. [group-feedback-synthesis.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/group-feedback-synthesis.md)
- Báo cáo tổng hợp đối chiếu chéo (Cross-Tester Synthesis) từ 4 phiên kiểm thử độc lập của 4 thành viên nhóm Tung Tung Tung Sahur.
- Ma trận phân tích First Action, Breakdown chính, Cách lấy lại control, Option được chọn và Trade-off cốt lõi.
- Quyết định Next Change thống nhất: Chọn Option A làm UI core, tích hợp Trigger khi sai Checkpoint từ Option C, tinh gọn chẩn đoán 1 câu từ Option B, sửa lỗi khóa cứng của Option C, và leo thang sang Option D khi sai từ 2 lần trở lên.

### 5. [ai-support-log.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/ai-support-log.md)
- Bảng nhật ký minh bạch theo quy chuẩn môn học phản ánh sự hợp tác giữa học viên và trợ lý AI trong suốt quy trình Day 19.
- Đánh giá thẳng thắn các sai lệch/hạn chế của AI và sự can thiệp thực tế của con người trong quá trình prototyping và user testing.
