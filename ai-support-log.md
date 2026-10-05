# NHẬT KÝ HỢP TÁC VÀ SỬ DỤNG TRỢ LÝ AI (AI SUPPORT LOG)
## DỰ ÁN VLEARN AI TUTOR: DIAGNOSTIC REFRESHER

> **Môn học:** AI Product Labs — Track 1 (Day 19: Prototyping & User Testing)  
> **Học viên thực hiện:** **Đỗ Lê Việt Anh** (MSSV: **2A202602491**) — Phụ trách chính: **Option B** (Chẩn đoán 3 câu)  
> **Nhóm thực hiện:** **Tung Tung Tung Sahur** (Lại Bá Quân, Đỗ Lê Việt Anh, Nguyễn Thị Minh Khánh, Nguyễn Quang Huy)  
> **Công cụ AI đã sử dụng:** Antigravity IDE (Gemini 3.8 Flash, Claude 3.5 Sonnet)

---

## 1. Bảng Nhật Ký Chi Tiết Hợp Tác Người & Máy (Detailed AI Collaboration Log)

| Giai đoạn / Tác vụ | AI đã hỗ trợ gì (Prompts & Output) | Điểm hạn chế, sai lệch hoặc hời hợt của AI | Cách con người can thiệp và hiệu chỉnh thực tế |
| :--- | :--- | :--- | :--- |
| **1. Lên ý tưởng 4 Phương án & Thiết kế Human–AI** | - Gợi ý cấu trúc bảng so sánh 4 options (A/B/C/D) theo các cấp độ tự chủ (Don't Act, Ask, Act, Suggest).<br>- Tạo khung bảng Human–AI Decision Table (Role & Agency, Expectation, Evidence & Uncertainty, Control & Recovery). | - AI ban đầu đề xuất các phương án chatbot chung chung dạng cửa sổ popup góc màn hình (Floating Widget), vi phạm nguyên tắc giữ sự tập trung in-context của bài học.<br>- Chưa bám sát hiện tượng người học bị nghẽn do thuật ngữ viết tắt trên slide. | - Can thiệp định hình lại 4 hướng tiếp cận tương phản rõ rệt: Option A (Chỉ vào chỗ kẹt - Quân), Option B (Chẩn đoán 3 câu - Việt Anh), Option C (AI tự nhắc - Khánh), Option D (Hỏi người thật - Huy).<br>- Chuẩn hóa 70% Shared Core trên 3 chủ đề kiến thức thực tế (`context`, `react`, `gd`). |
| **2. Xây dựng Nguyên mẫu tương tác (`prototype/index.html`)** | - Hỗ trợ sinh khung mã nguồn HTML/CSS/JS độc lập (zero dependencies), hỗ trợ hash navigation (`#/context/theory/A`).<br>- Viết hàm logger ghi nhận telemetry sự kiện (`start`, `quick-question`, `a-select`, `c-nudge`, `d-send`). | - AI có xu hướng import thư viện bên ngoài (Tailwind CDN, React bundle) khiến prototype cồng kềnh, dễ lỗi khi chạy offline không mạng.<br>- Logic chẩn đoán của Option B ban đầu bị AI viết cứng nhắc, không có đồ thị SVG trực quan. | - Yêu cầu thuần hóa 100% bằng Vanilla HTML/CSS/JS nhúng trong 1 file duy nhất để chạy mượt mà ngay trên mọi trình duyệt.<br>- Tự tay tinh chỉnh đồ thị SVG minh họa của Option B và bổ sung nút sao chép nhật ký CSV tại `#/log`. |
| **3. Soạn Kịch bản Kiểm thử & Chuẩn bị Test** | - Gợi ý dàn ý kịch bản điều phối Usability Testing theo giao thức Suy nghĩ thành lời (Think-Aloud Protocol).<br>- Đề xuất danh sách các câu hỏi gợi mở trung lập sau khi hoàn thành task. | - AI gợi ý một số câu hỏi mang tính định hướng chủ quan (ví dụ: *"Bạn có thấy Option C rất tiện lợi và thông minh không?"*). | - Loại bỏ toàn bộ câu hỏi mớm lời, thay bằng các quan sát hành vi khách quan: First action, thời gian dừng, các thao tác bấm nhầm/lúng túng và cách người học lấy lại quyền kiểm soát. |
| **4. Ghi chép & Phân tích phiên Test (Phiên 2 — Tester Thiều Quang Vinh)** | - Hỗ trợ chuẩn hóa định dạng nhật ký CSV 37 dòng xuất từ prototype logger.<br>- Định hình cấu trúc phân tích 4 lớp dữ liệu (Observed, Interpreted, Decided, Still Unproven). | - **AI hoàn toàn không thể tham gia vào phiên test thực tế:** AI không có mặt tại phòng 201 lúc 13:00, không nhìn thấy bạn Vinh bấm đáp án đúng trước rồi mới cố tình chọn sai để thử thách AI. | - Tự thân người nộp (Đỗ Lê Việt Anh) trực tiếp điều phối độc lập, bấm giờ, quan sát màn hình và ghi lại nguyên văn câu nói của tester về lỗi khóa cứng ở Option C.<br>- Tự rút ra bài học về hành vi "Reverse-testing" từ người học thật. |
| **5. Tổng hợp phản hồi nhóm & Chốt Next Change** | - Hỗ trợ tạo khung bảng ma trận đối chiếu chéo (Cross-Tester Synthesis) cho 4 phiên kiểm thử.<br>- Hỗ trợ tóm tắt các điểm tương đồng và khác biệt nổi bật. | - Khi đề xuất quyết định cải tiến tiếp theo, AI có xu hướng "tham lam" gộp tất cả các tính năng của cả 4 options vào một màn hình, làm mất đi sự tinh gọn ban đầu. | - Toàn nhóm Tung Tung Tung Sahur họp bàn và quyết định dứt khoát: Chọn Option A làm lõi tương tác, chỉ mượn cơ chế Trigger khi sai Quiz từ Option C, rút gọn chẩn đoán xuống 1 câu nhanh từ Option B, và chỉ dùng Option D khi làm sai liên tiếp 2 lần. |

---

## 2. Chiêm Nghiệm Cá Nhân Về Tương Tác Người & AI (Personal Reflection)

### 2.1. Đâu là thế mạnh lớn nhất của AI trong quy trình Prototyping?
- **Tốc độ hiện thực hóa mã nguồn (Rapid Code Scaffolding):** AI giúp biến ý tưởng thiết kế thành một nguyên mẫu web bấm được hoàn chỉnh (`prototype/index.html`) chỉ trong vài chục phút, với đầy đủ các trạng thái tương tác in-line card, side panel, modal và telemetry logger mà không cần dựng backend phức tạp.
- **Tính kỷ luật trong cấu trúc tài liệu:** AI hỗ trợ đắc lực trong việc giữ vững cấu trúc chuẩn mực (Human–AI Decision Matrix, 4-Layer Analysis, Cross-tester Synthesis), giúp các thành viên trong nhóm có cùng một ngôn ngữ trình bày nhất quán.

### 2.2. Đâu là giới hạn không thể thay thế của Con người (Human-in-the-Loop)?
1. **Nắm bắt hành vi phi tuyến tính của người dùng thật:** Không mô hình AI nào dự đoán được việc tester Thiều Quang Vinh khi vào bài sẽ ấn ngay vào đáp án đúng để xem output trước, rồi mới cố tình làm sai để kiểm tra xem AI nhảy ra ở đâu. Đây là sự tinh tế của tâm lý con người: người học muốn biết "chuẩn mực thành công" trông như thế nào trước khi thử nghiệm thất bại.
2. **Phát hiện Breakdown về cảm giác kiểm soát (Sense of Agency):** Khi bạn Vinh phát hiện sau khi được giải thích 1 đoạn thì không cho chọn tiếp các đoạn khác và thắc mắc *"Kể cả có hiểu hay không hiểu thì cũng phải cho người ta chọn tiếp chứ"*, đó là một trải nghiệm tâm lý về sự ức chế mà chỉ có con người quan sát trực tiếp mới thấu cảm trọn vẹn để đưa ra quyết định sửa đổi thiết kế.

### 2.3. Cam kết Liêm chính Học thuật (Academic Integrity Statement)
Tôi xác nhận rằng toàn bộ dữ liệu quan sát, các trích dẫn nguyên văn của bạn Thiều Quang Vinh, dữ liệu log 37 sự kiện và các phân tích trong hồ sơ nộp Day 19 đều xuất phát từ phiên làm việc thực tế do tôi trực tiếp thực hiện tại phòng 201 vào lúc 13:00 ngày 05/10/2026. Trợ lý AI chỉ đóng vai trò hỗ trợ dàn dựng mã nguồn nguyên mẫu và định dạng văn bản báo cáo.
