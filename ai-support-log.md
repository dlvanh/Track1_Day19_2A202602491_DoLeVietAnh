# NHẬT KÝ HỢP TÁC VÀ SỬ DỤNG TRỢ LÝ AI (AI SUPPORT LOG)
## DỰ ÁN UNIPILOT — HỆ ĐIỀU HÀNH TRỢ LÝ TUYỂN SINH THÔNG MINH ĐA TRƯỜNG (P-127)

> **Môn học:** AI Product Labs — Track 1 (Day 19: Prototyping & User Testing)  
> **Học viên thực hiện:** **Đỗ Lê Việt Anh** (MSSV: **2A202602491**)  
> **Nhóm thực hiện:** Nhóm P-127 (UniPilot Team)  
> **Công cụ AI đã sử dụng:** Antigravity IDE (Gemini 3.8 Flash, Claude 3.5 Sonnet), v0.dev (Generative UI Sandbox)

---

## 1. Bảng Nhật Ký Chi Tiết Hợp Tác Người & Máy (Detailed AI Collaboration Log)

| Giai đoạn / Tác vụ | AI đã hỗ trợ gì (Prompts & Output) | Điểm hạn chế, sai lệch hoặc hời hợt của AI | Cách con người can thiệp và hiệu chỉnh thực tế |
| :--- | :--- | :--- | :--- |
| **1. Lên ý tưởng 3 Phương án (Three-Option Exploration)** | - Gợi ý cấu trúc phân tích 3 hướng tiếp cận cho bài toán tư vấn tuyển sinh.<br>- Sinh khung bảng ma trận so sánh các tiêu chí đánh giá có trọng số. | - Ban đầu AI đề xuất các hướng generic của thương mại điện tử (e.g. *"Giỏ hàng nguyện vọng"*, *"Bộ lọc theo học phí rẻ"*).<br>- Bỏ qua đặc thù tâm lý lo âu tột độ và tính cạnh tranh điểm chuẩn khốc liệt của kỳ thi đại học tại Việt Nam. | - Tự tay định hình lại 3 phương án sát thực tế: **Chatbot widget** (phương án phổ thông), **Calm Counselor Desk** (phương án chủ lực bàn làm việc tĩnh) và **Diagnostic Wizard** (phương án khảo sát tuần tự).<br>- Tích hợp triết lý thiết kế từ `DESIGN_DIRECTION.md` (giấy ấm, mực tối, thước đo vị thế). |
| **2. Xây dựng Nguyên mẫu tương tác (Prototyping Setup)** | - Hỗ trợ sinh nhanh khung layout React/Tailwind cho thanh Thước đo vị thế (`AdmissionStanding.tsx`) trên v0.dev.<br>- Gợi ý cấu trúc bảng tra cứu điểm chuẩn lịch sử 2023–2025. | - AI sinh ra nhiều hiệu ứng màu mè (gradient lấp lánh, bo góc quá tròn, icon emoji ✨⚡ rực rỡ) vi phạm nguyên tắc *"A calm counselor's desk, not a dashboard"*.<br>- Công thức tính điểm xét tuyển AI tự sinh sai quy chế thực tế của ĐHQGHN. | - Loại bỏ 100% các gradient và icon trang trí thừa thãi; chuẩn hóa theo hệ màu đá ấm (`stone-200/900`) và `blue-700`.<br>- Tự tay cập nhật đúng công thức tính điểm chuẩn xác theo Đề án tuyển sinh Trường ĐH Công nghệ năm 2026. |
| **3. Soạn Kịch bản Kiểm thử (Facilitation Script & Tasks)** | - Gợi ý danh sách câu hỏi kiểm tra tính dễ dùng theo chuẩn Nielsen Norman Group.<br>- Tạo khung kịch bản mở đầu và kết thúc buổi thử nghiệm. | - Một số câu hỏi gợi ý của AI mang tính **mớm lời và định hướng lộ liễu** (ví dụ: *"Bạn có thấy giao diện này rất đẹp và dễ hiểu không?"*, *"Bạn có thích thanh thước đo màu vàng không?"*). | - Viết lại toàn bộ câu hỏi theo giao thức Suy nghĩ thành lời (**Think-Aloud Protocol**) và câu hỏi mở trung lập.<br>- Rút kinh nghiệm sâu sắc từ đợt phỏng vấn Day 17: Tuyệt đối không gợi ý chức năng hay khen chê sản phẩm trước mặt người dùng. |
| **4. Ghi chép & Phân tích phiên Test (Prototype Feedback Note)** | - Hỗ trợ chuẩn hóa định dạng bảng đo lường chỉ số định lượng (SEQ, SUS Score, Time-on-task).<br>- Hỗ trợ rà soát chính tả và cấu trúc biên bản ghi chép. | - **AI hoàn toàn không thể tham gia vào phiên test:** AI không nghe được giọng nói, không nhìn được nét mặt, không cảm nhận được tiếng thở dài hay sự lúng túng của người tham gia khi di chuột. | - Tự thân người nộp (Đỗ Lê Việt Anh) trực tiếp điều phối, quan sát, bấm giờ và ghi lại từng câu nói nguyên văn (quotes) của bạn Lê Hoàng Nam.<br>- Tự tính toán điểm SUS và viết phần chiêm nghiệm (reflection) từ trải nghiệm thật 100%. |
| **5. Tổng hợp phản hồi nhóm & Ma trận ưu tiên (Group Synthesis)** | - Gợi ý cấu trúc Ma trận ưu tiên Hành động (Impact vs. Effort Matrix) theo mô hình Eisenhower / MoSCoW. | - Khi yêu cầu AI phân loại các phản hồi, AI có xu hướng xếp mọi tính năng vào nhóm "Rất quan trọng - Cần làm ngay", gây phân tán nguồn lực của nhóm. | - Nhóm P-127 đã họp trực tiếp đối chiếu 4 biên bản kiểm thử; tự tay chọn lọc ra **chỉ 3 đầu việc P0 cốt lõi** cần sửa ngay cho giao diện frontend trước Demo Day (Font size footnote, Micro-copy nút Handoff, Reactive transition). |

---

## 2. Chiêm Nghiệm Cá Nhân Về Tương Tác Người & AI (Personal Reflection)

### 2.1. Đâu là thế mạnh lớn nhất của AI trong quy trình Prototyping?
- **Tốc độ cấu trúc hóa thông tin (Documentation Velocity):** AI đóng vai trò như một thư ký mẫn cán, giúp dàn dựng nhanh các khung tài liệu chuẩn mực quốc tế (Design Sheets, Usability Logs, Evaluation Tables), giúp giảm khoảng 60% thời gian gõ văn bản cơ bản để nhóm tập trung vào tư duy logic và thiết kế.
- **Tạo khung mã nguồn ban đầu (Code Scaffolding):** Công cụ AI hỗ trợ sinh nhanh khung component Tailwind/React để nhóm nhanh chóng có bản mẫu bấm được (clickable prototype) thay vì phải code từ con số không.

### 2.2. Đâu là giới hạn không thể thay thế của Con người (Human-in-the-Loop)?
1. **Sự thấu cảm người dùng sâu sắc (Empathy & Nuance):** AI không bao giờ hiểu được tâm lý của một học sinh 18 tuổi đang đứng trước bước ngoặt cuộc đời. Nỗi sợ vô hình khi bấm vào nút "Gặp cán bộ tư vấn" (vì sợ bị gọi điện thoại quấy rầy hoặc sợ bị đánh giá năng lực) là thứ chỉ có thể phát hiện qua ánh mắt ngập ngừng của người dùng thật trong phiên kiểm thử do chính tôi trực tiếp quan sát.
2. **Kiến thức thực chứng và Ngữ cảnh bản địa (Local Ground Truth):** AI không tự cập nhật được sự thay đổi tinh tế trong quy chế xét tuyển kết hợp của ĐHQGHN hay cách phụ huynh Việt Nam muốn gửi ảnh chụp màn hình qua Zalo. Nếu không có con người kiểm duyệt và chỉnh sửa nghiêm ngặt, câu trả lời của AI sẽ rất dễ rơi vào tình trạng "sáo rỗng kiểu phương Tây" hoặc sai lệch số liệu pháp lý.

### 2.3. Cam kết Liêm chính Học thuật (Academic Integrity Statement)
Tôi xác nhận rằng toàn bộ dữ liệu kiểm thử, biên bản quan sát, số liệu đo lường thời gian và các trích dẫn người dùng trong các tài liệu nộp của Day 19 đều xuất phát từ phiên làm việc thực tế do tôi và nhóm P-127 thực hiện. Trợ lý AI chỉ đóng vai trò hỗ trợ định dạng, đối chiếu cấu trúc và tăng tốc độ hoàn thiện tài liệu.
