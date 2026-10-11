# Bài làm: Thiết kế vận hành Scrum cho tính năng đặt xe ghép

## Phần 1: Phân tích nhịp Sprint

1. **Đầu vào và đầu ra của 1 Sprint:**
   - **Đầu vào:** Product Backlog đã được Product Owner làm rõ và sắp xếp ưu tiên, năng lực làm việc thực tế của nhóm Developers, cùng phản hồi từ bản tăng trưởng ở Sprint trước.
   - **Đầu ra:** Một bản tăng trưởng sản phẩm hoàn thành (Done Increment) đáp ứng Định nghĩa hoàn thành (Definition of Done), chạy được trên thực tế để người dùng thử nghiệm.

2. **Độ dài Sprint và số lượng Sprint trong 6 tuần:**
   - **Độ dài Sprint:** Cố định 2 tuần.
   - **Số lượng Sprint:** 3 Sprint trọn vẹn trong khoảng thời gian 6 tuần.

3. **Lý do lựa chọn gắn với trụ cột Scrum:**
   - Chu kỳ 2 tuần tạo ra các mốc cố định để người dùng và các bên liên quan trực tiếp thanh tra bản phần mềm chạy được tại buổi Sprint Review. Nhờ đó, đội phát hiện sớm các điểm lệch về trải nghiệm ghép chuyến và chia tiền, thay vì chờ đến cuối tuần thứ 6 mới nhận ra sản phẩm không khớp với nhu cầu thực tế.

---

## Phần 2: Thiết kế Product Backlog

| Thứ tự ưu tiên | Hạng mục công việc | Lý do ưu tiên |
| :---: | :--- | :--- |
| **1** | (a) Ghép khách đi cùng tuyến đường vào một chuyến | Đây là giá trị cốt lõi của tính năng xe ghép. Nếu hệ thống không tìm và ghép được khách chung hành trình, các nghiệp vụ tính tiền hay đánh giá phía sau đều không thể thực hiện. |
| **2** | (b) Tự động chia tiền cho từng khách trong chuyến | Khách chọn đi ghép với mục tiêu chính là tiết kiệm chi phí. Thuật toán chia tiền minh bạch giải quyết trực tiếp quyền lợi tài chính của khách ngay sau khi ghép chuyến thành công. |
| **3** | (c) Thanh toán bằng thẻ ngân hàng | Cần thiết để hoàn thiện luồng giao dịch khép kín không dùng tiền mặt. Hạng mục này xếp sau việc chia tiền vì trong giai đoạn thử nghiệm đầu, khách và tài xế vẫn có thể dựa vào số tiền chia tự động để thanh toán tiền mặt. |
| **4** | (d) Khách đánh giá bạn đi ghép sau mỗi chuyến | Tính năng bổ trợ nhằm nâng cao chất lượng dịch vụ và xây dựng văn hóa đi xe văn minh. Hạng mục này chỉ phát huy giá trị khi luồng ghép chuyến và thanh toán đã vận hành ổn định. |

---

## Phần 3: Xử lý yêu cầu thay đổi

Đức (Product Owner) là người tiếp nhận phản hồi từ khách và quyết định đưa tính năng thanh toán qua ví điện tử vào Product Backlog, xếp ở vị trí ưu tiên cao hơn thẻ ngân hàng. 

Đội Developers không đổi việc ngay lập tức mà giữ nguyên kế hoạch để hoàn thành mục tiêu của Sprint 1 đang chạy dở. 

Yêu cầu thanh toán qua ví điện tử sẽ chính thức được đưa vào lựa chọn và phân chia nhiệm vụ tại buổi Sprint Planning của Sprint 2.
