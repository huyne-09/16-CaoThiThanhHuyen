# Trả lời Câu 2: Các sự kiện trong một Sprint của Scrum



**a.**

Một Sprint trong Scrum bao gồm 4 sự kiện chính:

1. **Sprint Planning (Lập kế hoạch Sprint):**
    * **Mục đích:** Đây là sự kiện diễn ra đầu tiên. Toàn bộ Nhóm Scrum (Scrum Team) cùng nhau thảo luận và quyết định công việc sẽ được thực hiện trong Sprint này.
    * **Kết quả:** Tạo ra **Sprint Backlog** – là danh sách các mục (User Stories) được chọn từ Product Backlog và một kế hoạch chi tiết (các task) để hoàn thành chúng.

2. **Daily Scrum (Scrum Hàng ngày):**
    * **Mục đích:** Là một cuộc họp ngắn (tối đa 15 phút) diễn ra mỗi ngày cho Nhóm Phát triển (Developers). Mục tiêu là để đồng bộ công việc, kiểm tra tiến độ so với mục tiêu Sprint và điều chỉnh kế hoạch cho 24 giờ tới.
    * **Nội dung:** Các thành viên thường trả lời 3 câu hỏi: "Hôm qua đã làm gì?", "Hôm nay sẽ làm gì?", và "Có gặp khó khăn (trở ngại) gì không?".

3. **Sprint Review (Sơ kết Sprint):**
    * **Mục đích:** Diễn ra vào cuối Sprint. Nhóm Phát triển trình bày sản phẩm (Increment) mà họ đã hoàn thành cho Product Owner và các bên liên quan (stakeholders).
    * **Kết quả:** Thu thập phản hồi, góp ý về sản phẩm. Dựa trên phản hồi này, Product Owner có thể điều chỉnh Product Backlog cho các Sprint tương lai.

4. **Sprint Retrospective (Cải tiến Sprint):**
    * **Mục đích:** Đây là sự kiện *cuối cùng* trong Sprint. Toàn bộ Nhóm Scrum (kể cả Product Owner và Scrum Master) họp nội bộ để nhìn lại toàn bộ quy trình làm việc trong Sprint vừa qua.
    * **Kết quả:** Tìm ra những gì đã làm tốt, những gì chưa tốt, và đưa ra các hành động cụ thể để cải tiến quy trình làm việc trong Sprint tiếp theo.

---

**b**

Buổi Sprint Planning cho User Story (US) này sẽ diễn ra như sau:

1. **Làm rõ Yêu cầu (What):**
    * Product Owner (PO) trình bày US: "Là một người dùng, tôi muốn tạo một ghi chú mới".
    * Nhóm Phát triển (Dev Team) sẽ đặt câu hỏi cho PO để làm rõ yêu cầu (Acceptance Criteria - Tiêu chí chấp nhận):
        * "Người dùng nhấn vào nút nào để 'tạo'?"
        * "Một 'ghi chú mới' bao gồm những gì? (Chỉ có nội dung, hay có cả Tiêu đề?)"
        * "Có giới hạn ký tự không?"
        * "Sau khi tạo xong, ghi chú sẽ hiển thị ở đâu (đầu danh sách, cuối danh sách)?"
        * "Có cần chức năng 'Lưu' (Save) hay ứng dụng tự động lưu (Auto-save)?"

2. **Phân rã công việc (How):**
    * Sau khi hiểu rõ yêu cầu, Nhóm Phát triển sẽ cùng nhau phân rã (breakdown) US này thành các công việc kỹ thuật (Task) cụ thể.
    * **Ví dụ các Task:**
        * *Task 1:* Thiết kế giao diện (UI) cho màn hình "Tạo ghi chú mới" (vd: 1 ô Tiêu đề, 1 ô Nội dung, 1 nút "Lưu").
        * *Task 2:* Lập trình (code) giao diện Front-end cho màn hình này.
        * *Task 3:* Cập nhật/Thiết kế Cơ sở dữ liệu (Database) để lưu trữ ghi chú (vd: tạo bảng `Notes`).
        * *Task 4:* Viết API (Back-end) cho chức năng "Lưu ghi chú" (nhận dữ liệu từ Front-end và lưu vào Database).
        * *Task 5:* Kết nối nút "Lưu" ở Front-end để gọi API Back-end.
        * *Task 6:* Viết Kịch bản kiểm thử (Test Case) cho chức năng "Tạo ghi chú mới".
        * *Task 7:* Thực hiện kiểm thử (Testing) chức năng.

3. **Ước tính (Estimation):**
    * Nhóm Phát triển sẽ ước lượng thời gian (ví dụ: theo giờ) hoặc độ phức tạp (ví dụ: theo điểm - Story Point) cần thiết để hoàn thành *từng Task* đã vạch ra ở trên.

4. **Cam kết (Commitment):**
    * Sau khi phân rã và ước tính, Nhóm Phát triển xác nhận rằng họ có đủ khả năng (capacity) để hoàn thành User Story này trong Sprint. User Story này và các Task liên quan chính thức được đưa vào **Sprint Backlog**.
