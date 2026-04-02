---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:
- Nghiên cứu và tích hợp mô hình ngôn ngữ lớn (LLM) trong vai trò công tắc phòng vệ (Fallback).
- Sử dụng Google Gemini / Amazon Bedrock đọc hóa đơn nhòe nát, tùy biến cấu trúc.
- Thiết kế luồng tạo Prompt AI tương tác đa phương thức (Multi-modal).

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc |
| --- | --- |
| 2 | - Bắt mạch lỗi các Edge Cases khiến cho model local LayoutLM bó tay (hóa đơn viết tay, chữ in kim than bị bay mực hoàn toàn). |
| 3 | - Nghiên cứu ứng dụng đa phương tiện (Multi-modal) của LLM. <br> - Lấy API Keys của Gemini Flash / thiết lập Amazon Bedrock (sử dụng Anthropic Claude). |
| 4 | - Đi sâu vào Prompt Engineering. Thiết kế một siêu Prompt hướng dẫn LLM phân tích hình ảnh và ói ra cấu trúc JSON chuẩn mapping với local schema. |
| 5 | - Viết luồng Fallback: Nếu ảnh xử lý từ mô hình local báo Confidence < 80% -> Bắn thẳng payload Ảnh + Prompt lên LLM để LLM đọc giúp. |
| 6 | - **Thực hành:** <br>&emsp; + Giải phẫu chức năng Fallback bằng 50 hóa đơn siêu mờ và nhiễu <br>&emsp; + Nhận diện tình trạng LLM bị ảo giác (Hallucination) và bẻ lái hạn chế nó bằng system prompt chặt chẽ hơn. |

### Kết quả đạt được tuần 9:

- Tích hợp thành công GenAI vào quy trình xử lý giải cứu các ca rớt mạng làm giảm hẳn tỉ lệ nhận diện sai vặt.
- Có level nâng cao về Prompt Engineering ép LLM ói ra kết quả JSON chuẩn xác.
- Xây dựng được kiến trúc OCR hai lớp tinh vi (Local tiết kiệm chi phí + Cloud LLM siêu sức mạnh).

