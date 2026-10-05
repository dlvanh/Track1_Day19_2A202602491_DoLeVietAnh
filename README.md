# BÀI NỘP TRACK 1 — DAY 19: PROTOTYPING & USER TESTING
## DỰ ÁN UNIPILOT — HỆ ĐIỀU HÀNH TRỢ LÝ TUYỂN SINH THÔNG MINH ĐA TRƯỜNG (P-127)

> **Khóa học:** AI20K Bootcamp — Cohort 4  
> **Học phần:** Track 1: AI Product Labs (AI Product Design & Prototyping)  
> **Học viên:** **Đỗ Lê Việt Anh**  
> **Mã số sinh viên (MSSV):** **2A202602491**  
> **Nhóm thực hiện:** **Nhóm P-127 (UniPilot Team)**  
> **Đơn vị thí điểm:** Trường Đại học Công nghệ – ĐHQGHN (UET - VNU)  
> **Ngày hoàn thành bài nộp:** 05/10/2026

---

## 📂 Danh Mục 5 Hồ Sơ Bàn Giao (Deliverables Structure)

```
Track1_Day19_2A202602491_DoLeVietAnh/
├── three-option-design-sheet.md       # Bảng phân tích 3 phương án thiết kế A/B/C & link Figma board
├── prototype-link.md                  # Danh sách liên kết nguyên mẫu tương tác A/B/C chung của nhóm
├── prototype-feedback-note.md         # Biên bản chi tiết phiên kiểm thử thực tế do chính Việt Anh điều phối
├── group-feedback-synthesis.md        # Báo cáo tổng hợp phản hồi toàn nhóm & ma trận ưu tiên P0/P1/P2
└── ai-support-log.md                  # Nhật ký minh bạch sử dụng AI & phản biện của con người
```

---

## 📌 Tóm Tắt Nội Dung Từng Tài Liệu

### 1. [three-option-design-sheet.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/three-option-design-sheet.md)
- Phân tích chi tiết 3 hướng tiếp cận thiết kế giải quyết bài toán tư vấn tuyển sinh:
  - **Phương án A:** *Conversational Floating Widget* (Chatbot góc màn hình truyền thống).
  - **Phương án B:** *"Calm Counselor's Desk"* (Bàn tư vấn tĩnh lặng với Thước đo vị thế `AdmissionStanding` & Trợ lý trích dẫn Footnote pháp lý) — **Phương án được chọn làm lõi**.
  - **Phương án C:** *Diagnostic Wizard* (Bộ câu hỏi khảo sát 4 bước trắc nghiệm).
- Ma trận so sánh 5 tiêu chí có trọng số (Khả năng giải tỏa lo âu, Độ tin cậy tri thức, Tốc độ, Hiệu quả giảm tải cán bộ, Tính khả thi kỹ thuật).
- Đính kèm liên kết Figma Design Sprint Board chung của nhóm.

### 2. [prototype-link.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype-link.md)
- Tổng hợp đầy đủ đường dẫn trải nghiệm trực tiếp 3 nguyên mẫu (Cloud sandbox, Vercel preview, Figma click-through).
- Hướng dẫn truy cập phân hệ Thí sinh (`/candidate`) và phân hệ Cán bộ tư vấn (`/consultant`).
- Cung cấp tài khoản thử nghiệm và hướng dẫn khởi chạy nguyên mẫu trên máy cục bộ (`npm run dev`).

### 3. [prototype-feedback-note.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype-feedback-note.md)
- Biên bản ghi chép phiên kiểm thử định tính 1-1 có hướng dẫn (Moderated Usability Testing) do chính **Đỗ Lê Việt Anh** điều phối.
- Người tham gia: Bạn Lê Hoàng Nam (18 tuổi, Học sinh lớp 12 chuyên Tin - THPT Chuyên KHTN, nguyện vọng vào ngành CNTT CN1 của UET).
- Ghi nhận chi tiết diễn biến từng phút của 3 nhiệm vụ kiểm thử kèm các câu nói trực tiếp (quotes) giàu cảm xúc.
- Đo lường chỉ số định lượng: Completion Rate 100%, SUS Score **85.0/100 (Hạng A)**, SEQ từng task.
- Chiêm nghiệm cá nhân của người điều phối và 3 hành động kỹ thuật tinh chỉnh frontend tức thì.

### 4. [group-feedback-synthesis.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/group-feedback-synthesis.md)
- Báo cáo tổng hợp dữ liệu từ 4 phiên kiểm thử của nhóm P-127 trên 4 nhóm chân dung người dùng (Thí sinh chuyên, Thí sinh tỉnh, Phụ huynh học sinh, Cán bộ tuyển sinh).
- 4 cụm phát hiện cốt lõi: Giá trị của Visual Anchor (Thước đo điểm), Tính pháp lý của Footnotes, Nỗi e ngại khi gặp nút Handoff, và Giá trị tiết kiệm thời gian của Thẻ tóm tắt hồ sơ đối với cán bộ.
- Ma trận ưu tiên hành động (Impact vs. Effort): Phân định rõ ràng các hạng mục P0, P1, P2 trước thềm Demo Day.
- Quyết định phê duyệt 100% kiến trúc Phương án B của toàn đội.

### 5. [ai-support-log.md](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/ai-support-log.md)
- Bảng nhật ký minh bạch theo quy chuẩn môn học với 4 cột: Tác vụ, Đóng góp của AI, Giới hạn/Sai lệch của AI, Can thiệp thực tế của con người.
- Phản ánh rõ ràng vai trò hỗ trợ của AI (tăng tốc dàn khung tài liệu) và giá trị không thể thay thế của con người (thấu cảm người dùng, nắm bắt tâm lý lo âu kỳ thi, am hiểu quy chế tuyển sinh Việt Nam).
