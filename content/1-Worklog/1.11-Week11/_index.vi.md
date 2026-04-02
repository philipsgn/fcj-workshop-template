---
title: "Worklog Tuần 11"
date: 2024-01-01
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu tuần 11:
- Triển khai bộ quy tắc xác thực toán học tự kiểm lỗi sai.
- Phát triển bộ điểm tin cậy nhằm cảnh báo nhân sự kiểm tra lại (Human-in-the-loop).
- Giấu kín Key cấu hình và biến môi trường quan trọng bằng AWS Secrets Manager.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Xây hàm 'Math Validation' tự động: Tổng tiền bắt buộc = (Đơn giá x Số lượng) + Thuế. <br> - Đưa ra quy định ứng phó nếu thuật toán AI đọc sai một con số làm lệch phép tính. |
| 3 | - Thang đo điểm tin cậy (Confidence Score): Thuật toán phải tự phản hồi xem nó tự tin bao nhiêu % với con số vừa trích xuất. <br> - Trả về mã màu cảnh báo (Blue/Yellow/Red) để user dễ dòm lỗi. |
| 4 | - Thanh tra toàn bộ file codebase: Quét và loại bỏ sạch LLM API Keys hoặc Password CSDL vô tình code cứng dưới dạng String. |
| 5 | - Học cách sử dụng AWS Systems Manager Parameter Store và AWS Secrets Manager. <br> - Upload các token, key bảo mật tuyệt đối vô két sắt của AWS Secrets Manager. |
| 6 | - **Thực hành:** <br>&emsp; + Chỉnh sửa ECS Task Definition để tự móc nối mật khẩu từ ARN Cloud lúc mới boot lên thay vì lấy qua biến file text <br>&emsp; + Đảm bảo app vẫn chạy siêu nuột nà dù source code không hề lộ khóa. |

### Kết quả đạt được tuần 11:

- Đưa khả năng chống chịu lỗi của AI lên tầm cỡ Production nhờ việc tự động vá lỗi bằng giải thuật kiểm tra chéo (Math Cross-check).
- Tích hợp hoàn hảo thao tác xét duyệt thủ công (Human-in-the-loop) dựa theo phân luồng trạng thái từ điểm tin cậy.
- Đạt tiêu chuẩn bảo mật cho cấu hình Backend không thể bị hack với AWS Secrets Manager.

