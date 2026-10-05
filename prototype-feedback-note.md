# PROTOTYPE FEEDBACK NOTE (CÁ NHÂN)
## DỰ ÁN VLEARN AI TUTOR: DIAGNOSTIC REFRESHER

> **Khóa học:** AI20K Bootcamp — Cohort 4  
> **Học phần:** Track 1: AI Product Labs (Day 19: Prototyping & User Testing)  
> **Người thực hiện facilitate & ghi chép:** **Đỗ Lê Việt Anh** (MSSV: **2A202602491**)  
> **Phương án phụ trách chính:** **Option B** (Chẩn đoán 3 câu — Diagnostic Micro-Check & Knowledge Gap Triage)  
> **Nhóm thực hiện:** **Tung Tung Tung Sahur**  
> **Thành viên nhóm:** Lại Bá Quân (Lead Opt A), Đỗ Lê Việt Anh (Lead Opt B), Nguyễn Thị Minh Khánh (Lead Opt C), Nguyễn Quang Huy (Lead Opt D)  
> **Case Study:** Hỗ trợ người học vượt qua điểm nghẽn kiến thức trên nền tảng VLearn  
> **Nguyên mẫu kiểm thử:** [`prototype/index.html`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype/index.html)  
> **Hồ sơ liên quan:** [`three-option-design-sheet.md`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/three-option-design-sheet.md) | [`group-feedback-synthesis.md`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/group-feedback-synthesis.md) | [`prototype-link.md`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype-link.md)  
> **Quy định**: Phiên này do chính bạn trực tiếp điều phối độc lập với 1 tester ngoài nhóm. Tester được trải nghiệm ĐỦ CẢ 4 OPTIONS (A, B, C, D) trên cùng một chủ đề bài học và cùng một Outcome Task.

---

## 1. THÔNG TIN PHIÊN TEST
- **Tester (Tên viết tắt / Mã):** **Tester 2 (Phiên 2)** — **Thiều Quang Vinh** (MHV: **2A202602877**, Học viên AI Thực Chiến khóa 4)
- **Bối cảnh thực tế (Relevant Context):** Khi học lý thuyết trên VLearn, bạn có thói quen khi vào bài là bấm ngay vào đáp án đúng của câu hỏi nhanh (Quiz) để xem output hệ thống phản hồi những gì trước. Sau đó bạn bấm làm lại và cố tình chọn đáp án sai để kiểm tra xem AI sẽ nhảy ra hỗ trợ ở đâu và giúp được những gì.
- **Chủ đề test:** Context Window (Slide 12 · Lý thuyết) — URL khởi động: [`prototype/index.html#context/theory/A`](file:///d:/AI20K/Track1_Day19_2A202602491_DoLeVietAnh/prototype/index.html#context/theory/A)
- **Thời gian & Địa điểm:** **13:00 – 13:15 ngày 05/10/2026, thực hiện trực tiếp tại phòng học 201**.
- **Thứ tự trải nghiệm các options:** **Option A ➔ Option C ➔ Option D ➔ Option C (kiểm tra lại tương tác sâu)**

---

## 2. BẢNG GHI NHẬN HÀNH VI (OBSERVATION LOG)

| Tiêu điểm quan sát | Ghi nhận chi tiết trong lúc test |
| :--- | :--- |
| **First Action** *(Hành động đầu tiên họ làm khi thấy màn hình: đọc bài, bấm nút `Tôi vẫn chưa hiểu`, hay làm câu hỏi nhanh)* | Khi vừa vào màn hình, tester cuộn ngay xuống phần câu hỏi nhanh và **bấm chọn đáp án ĐÚNG trước** (chọn *"Bản tóm tắt bị cắt giữa chừng"*) để xem output hiển thị gì khi làm đúng (t=14s ở Opt A, t=10s ở Opt C). Sau đó bấm "Làm lại" và **cố tình chọn đáp án SAI** (chọn *"Không sao, 8.000 token chỉ tính cho input"*) để quan sát xem AI giúp được những gì và xuất hiện ở đâu. |
| **Chỗ dừng, do dự hoặc hiểu sai** *(Điểm khựng lại, bấm nhầm, ngập ngừng)* | **Breakdown chính:** Khi trải nghiệm Option C (lúc 13:10), tester phát hiện: **khi đã chọn được 1 đoạn/khái niệm và được AI xuất thẻ giải thích rồi thì hệ thống không cho chọn tiếp các phần còn lại để giải thích (kể cả có hiểu hay không)**; ở Option D tester ngập ngừng mở modal 2 lần nhưng đều hủy bỏ sau vài giây vì không muốn làm phiền người thật. |
| **Evidence & Uncertainty** *(Họ có đọc giải thích/căn cứ "Vì sao AI nghĩ vậy", trích dẫn nguồn, thước đo độ chắc chắn không?)* | Có đọc kỹ thẻ giải thích của AI. Ở Option A đọc xong bấm *"Đã rõ hơn"* (`understood`) cho cả 2 đoạn `token` và `memory`. Ở Option C, khi làm sai câu hỏi nhanh và thấy AI tự nudge thẻ `budget`, bạn đọc kỹ phần giải thích rồi bấm *"Đúng chỗ, đã rõ hơn"* (`c-accept`). |
| **Cách tester sửa sai hoặc lấy lại control** *(Nút Làm lại, Đóng ×, Bỏ qua, Tắt tự nhắc, Không đúng chỗ họ dùng thế nào?)* | Bấm nút *"Làm lại"* trên prototype bar; bấm nút *"Đóng ×"* (`a-close`) để tắt thẻ in-line card; bấm hủy modal ở Option D (`d-cancel-draft`); bấm nút **"Không đúng chỗ"** (`c-reject "budget"`) ở Option C để từ chối gợi ý của AI và tìm cách tự chọn đoạn khác. |
| **Option được chọn cuối cùng** | **Option C** (Được nhận xét là dùng **trực quan nhất** trong 4 phương án của nhóm) |
| **Lý do lựa chọn & Trade-off** *(Họ thích điểm gì và chấp nhận đánh đổi điều gì?)* | **Thích nhất:** Chọn được đúng chỗ mình chưa hiểu để AI giải thích tại chỗ, giao diện trực quan và khoanh vùng rất rõ ràng; **Trade-off:** Chấp nhận **không có đánh đổi gì cả** (thấy phương án này tiện lợi và thông minh nhất). |
| **Evidence đi ngược lại kỳ vọng của nhóm** *(Điểm gì tester làm khiến nhóm bất ngờ?)* | Nhóm bất ngờ trước hành vi kiểm thử chủ động 2 chiều của tester: làm đúng trước để xem kết quả chuẩn, rồi mới cố tình làm sai để kiểm tra cơ chế cứu hộ của AI; ngoài ra tester mở Option D đến 2 lần nhưng đều đóng ngay lập tức (`d-cancel-draft`) chứng minh người học rất e ngại bấm gửi yêu cầu cho người thật khi tự học lý thuyết ngắn. |

---

## 3. PHÂN TÍCH 4 LỚP DỮ LIỆU (FOUR-LAYER ANALYSIS)

### 1. OBSERVED (Dữ liệu quan sát khách quan)
*Dán dữ liệu nhật ký CSV trích xuất từ nút `Facilitator log` ➔ `Copy dạng CSV` của prototype vào đây:*
```csv
time,option,t_sec,event,detail
13:02:19,A·context/LT,0,start,""
13:02:33,A·context/LT,14,quick-question,"đúng (lần 1, chọn ""Bản tóm tắt bị cắt giữa chừng"")"
13:02:35,A·context/LT,16,done,"câu hỏi nhanh: 1 lần"
13:02:39,A·context/LT,0,start,""
13:02:55,A·context/LT,16,quick-question,"sai (lần 1, chọn ""Không sao, 8.000 token chỉ tính cho input"")"
13:02:58,A·context/LT,19,open-help,"sau câu hỏi nhanh"
13:03:04,A·context/LT,25,a-select,"+token"
13:03:08,A·context/LT,29,a-send,"chọn=[token] kiểu=explain sửa_tay=false → token"
13:03:21,A·context/LT,42,understood,"token"
13:03:23,A·context/LT,44,open-help,"sau câu hỏi nhanh"
13:03:25,A·context/LT,46,a-select,"+token"
13:03:27,A·context/LT,47,a-send,"chọn=[token] kiểu=explain sửa_tay=false → token"
13:03:35,A·context/LT,55,a-close,""
13:03:39,A·context/LT,59,open-help,"sau câu hỏi nhanh"
13:03:40,A·context/LT,61,a-select,"+memory"
13:03:41,A·context/LT,62,a-send,"chọn=[memory] kiểu=explain sửa_tay=false → memory"
13:04:11,A·context/LT,92,understood,"memory"
13:04:13,A·context/LT,94,open-help,"sau câu hỏi nhanh"
13:04:23,C·context/LT,0,start,""
13:04:33,C·context/LT,10,quick-question,"đúng (lần 1, chọn ""Bản tóm tắt bị cắt giữa chừng"")"
13:04:38,C·context/LT,15,done,"câu hỏi nhanh: 1 lần"
13:04:41,C·context/LT,0,start,""
13:04:43,C·context/LT,2,quick-question,"sai (lần 1, chọn ""Không sao, 8.000 token chỉ tính cho input"")"
13:04:43,C·context/LT,2,c-nudge,"sau khi sai câu hỏi nhanh"
13:04:54,C·context/LT,13,c-accept,"budget"
13:05:07,C·context/LT,26,open-help,"sau câu hỏi nhanh"
13:05:12,C·context/LT,32,quick-question,"đúng (lần 2, chọn ""Bản tóm tắt bị cắt giữa chừng"")"
13:05:13,C·context/LT,33,done,"câu hỏi nhanh: 2 lần"
13:05:17,D·context/LT,0,start,""
13:05:19,D·context/LT,2,open-help,"từ nội dung"
13:05:28,D·context/LT,11,d-cancel-draft,""
13:05:30,D·context/LT,13,open-help,"từ nội dung"
13:05:31,D·context/LT,15,d-cancel-draft,""
13:05:33,D·context/LT,16,quick-question,"đúng (lần 1, chọn ""Bản tóm tắt bị cắt giữa chừng"")"
13:10:34,C·context/LT,0,start,""
13:10:37,C·context/LT,3,open-help,"từ nội dung"
13:10:42,C·context/LT,8,c-reject,"budget"
```

*Ghi lại chính xác những gì tester đã nói (nguyên văn quotes) và các thao tác thực tế họ đã click:*
- **Thao tác thực tế tại phòng 201:** 
  - **Option A (13:02:19 – 13:04:13):** Bấm làm đúng câu hỏi nhanh ở giây 14 $\rightarrow$ hoàn tất. Bấm làm lại ở giây 20, chọn đáp án sai $\rightarrow$ bấm nút *"Tôi vẫn chưa hiểu"* $\rightarrow$ chạm chọn khối `token`, bấm gửi $\rightarrow$ đọc xong bấm *"Đã rõ hơn"*. Mở tiếp trợ giúp lần 2 và lần 3 để chọn tiếp khối `memory` $\rightarrow$ bấm gửi $\rightarrow$ đọc xong bấm *"Đã rõ hơn"*.
  - **Option C (13:04:23 – 13:05:13):** Bấm làm đúng câu hỏi nhanh ở giây 10 $\rightarrow$ hoàn tất. Bấm làm lại, chọn sai ở giây thứ 2 $\rightarrow$ AI tự động kích hoạt `c-nudge` ghim vào đoạn `budget` ngay lập tức $\rightarrow$ tester đọc và bấm *"Đúng chỗ, đã rõ hơn"* (`c-accept`) $\rightarrow$ làm lại câu hỏi nhanh và chọn đúng.
  - **Option D (13:05:17 – 13:05:33):** Bấm mở nút trợ giúp mở modal 2 lần nhưng đều bấm hủy (`d-cancel-draft`) chỉ sau vài giây $\rightarrow$ quay lại làm đúng câu hỏi nhanh trong 16s.
  - **Option C kiểm tra lại (13:10:34 – 13:10:42):** Mở lại Option C từ nội dung, khi AI tự đề xuất thẻ `budget` thì bấm *"Không đúng chỗ"* (`c-reject`) để kiểm tra xem hệ thống cho làm gì tiếp theo, và phát hiện ra việc không cho chọn tiếp các đoạn khác.
- **Lời nói / Trích dẫn trực tiếp của bạn Thiều Quang Vinh:**
  > *"Để em ấn thử vào đáp án đúng trước xem output nó hiện ra cái gì đã."*  
  > *"Rồi, bây giờ làm sai thử xem AI nó sẽ nhảy ra giúp mình ở đâu và giúp được những gì."*  
  > *"Ủa sao cái C này khi mình chọn được 1 cái và được AI giải thích rồi thì không được chọn mấy cái kia để giải thích nữa anh? Kể cả có hiểu hay không hiểu thì cũng phải cho người ta chọn tiếp chứ."*  
  > *"Trong mấy cái thì em thấy phương án C là dùng trực quan nhất, nhìn vào biết ngay mình sai ở đâu, không phải đánh đổi gì cả."*

### 2. INTERPRETED (Diễn giải ý nghĩa)
*Nhóm/bạn phỏng đoán hành vi trên thể hiện tâm lý hay trở ngại gì của người dùng:*
- **Hành vi "Reverse-testing" (Kiểm thử ngược từ đích):** Tester coi câu hỏi kiểm tra (Checkpoint) là mỏ neo trung tâm. Người học muốn xem phản hồi khi thành công trước, sau đó mới thử nghiệm nhánh thất bại để đánh giá năng lực của AI. Điều này chứng minh nút kích hoạt AI phải gắn liền với kết quả câu hỏi kiểm tra.
- **Nhu cầu tương tác đa khối (Multi-block Exploration):** Việc tester thử cả `token` lẫn `memory` ở Option A và bấm thử `c-reject` ở Option C cho thấy người học không chỉ kẹt ở một khái niệm duy nhất; họ có nhu cầu đối chiếu chéo nhiều khái niệm liên quan. Khi AI khóa lại chỉ cho giải thích 1 lần, người học cảm thấy bị mất quyền kiểm soát (loss of control).
- **Rào cản tâm lý của Option D:** Thao tác mở modal rồi bấm hủy 2 lần liên tiếp (`d-cancel-draft` lúc 13:05:28 và 13:05:31) cho thấy người học chỉ tò mò xem giao diện người thật hoạt động thế nào; khi thấy phải soạn nội dung gửi đi, họ lập tức hủy bỏ vì không muốn làm phiền Mentor cho một câu hỏi lý thuyết ngắn.

### 3. DECIDED — NEXT CHANGE (Đề xuất thay đổi)
*Từ phát hiện của phiên này, bạn đề xuất nhóm nên sửa đổi, giữ lại hoặc loại bỏ chi tiết nào trong thiết kế:*
- **Thay đổi 1 (Khắc phục triệt để breakdown của Option C):** Sau khi người học bấm *"Đúng chỗ, đã rõ hơn"* hoặc *"Không đúng chỗ"*, hệ thống không được khóa cứng mà phải hiển thị thêm tùy chọn: *"Bạn có muốn tìm hiểu thêm đoạn nào khác trên slide này không?"* hoặc mở lại chế độ chạm chọn của Option A.
- **Thay đổi 2 (Trigger thông minh theo Checkpoint):** Tận dụng điểm mạnh của Option C: khi người học trả lời sai câu hỏi nhanh, tự động hiển thị thẻ gợi ý khoanh vùng đúng đoạn bị hổng kiến thức mà không cần người học phải tự mày mò tìm kiếm.
- **Thay đổi 3 (Đơn giản hóa Option D):** Giữ Option D làm phao cứu sinh cuối cùng khi người học làm sai quá 2 lần, không hiển thị quá sớm làm người học phân tâm.

### 4. STILL UNPROVEN (Điều vẫn chưa thể khẳng định)
*Nhận thức rõ giới hạn của 1 phiên test: Điều gì vẫn cần thêm dữ liệu để chứng minh?*
- **Tác động của môi trường kiểm thử trực tiếp:** Buổi test diễn ra trực tiếp tại lớp 201 giữa giờ học, tester có tâm lý thoải mái và chủ động "thử nghiệm" tính năng. Vẫn chưa khẳng định được khi người học ngồi một mình lúc đêm muộn bị deadline dí thì họ có đủ kiên nhẫn để thử các phương án hay sẽ copy thẳng sang ChatGPT ngoài.
- **Khả năng áp dụng trên bài Lab thực hành:** Tester mới thử nghiệm trên Slide lý thuyết 12. Cần thêm dữ liệu kiểm thử trên bài Lab (Task 2 về `trim_history`) khi code chạy báo lỗi runtime để xem tính trực quan của Option C có giải quyết được lỗi code hay không.