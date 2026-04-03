---
title: "Tự đánh giá"
date: 2024-01-01
weight: 5
chapter: false
pre: " <b> 5. </b> "
---

Trong suốt thời gian thực tập với dự án SmartInvoice Shield từ tháng 1/2026 đến tháng 4/2026, tôi đã có cơ hội học hỏi và áp dụng các công nghệ AI tiên tiến cùng dịch vụ AWS Cloud vào một hệ thống quản lý hóa đơn thực tế.
Tôi đã trực tiếp tham gia nghiên cứu, xây dựng và tối ưu hóa luồng lõi AI OCR (AI OCR pipeline), tích hợp mượt mà với team Backend để đưa hệ thống vào môi trường Production.

### Các Đóng Góp Chính & Điểm Nhấn Kỹ Thuật

**1. Phát triển Kiến trúc AI & Mô hình Nhận diện (AI Model Development)**
- Trực tiếp tham gia thiết kế kiến trúc nhận diện đa tầng (Multi-tier AI OCR), ứng dụng mạnh mẽ **Gemini API** làm động cơ trích xuất dữ liệu hóa đơn linh hoạt và chuẩn xác.
- Triển khai và huấn luyện mô hình **LayoutLMv3** để máy học cách đọc hiểu theo cấu trúc (layout-aware), đồng thời kết hợp **PaddleOCR + VietOCR** tạo thành luồng dự phòng (Backup Pipeline) có độ chính xác cao và tối ưu chi phí.
- Xây dựng một **Rule Engine** (Động cơ xử lý luật) khắt khe ở bước hậu xử lý nhằm kiểm tra chéo độ tin cậy dữ liệu (như đối chiếu phép tính tổng tiền) trước khi trả JSON về cho Backend.

**2. Triển khai Đám mây (AWS) & Tích hợp Hệ thống**
- Với vai trò AI Engineer, tôi trực tiếp chuẩn hóa, đóng gói (Containerization) các mô hình AI để tích hợp mượt mà với hệ thống Backend .NET 9 trên nền tảng AWS ECS Fargate Spot.
- Phối hợp chặt chẽ với Backend Lead để giải quyết bài toán xử lý bất đồng bộ, đảm bảo luồng AI có thể nhận và giải quyết triệt để các payload hóa đơn xếp hàng trong Amazon SQS.
- Kiểm soát và tối ưu chi phí suy luận (Inference costs) thông qua việc điều hướng linh hoạt số lượng API calls giữa Gemini và mô hình On-premise (LayoutLMv3/PaddleOCR).

**3. Tối ưu Hệ thống & Xử lý Sự cố (Troubleshooting)**
- Giải quyết thành công các vấn đề liên quan đến độ trễ (OCR Latency) bằng cách tối ưu hóa các điều kiện rẽ nhánh mô hình dựa trên điểm tin cậy (Confidence score).
- Nghiên cứu và giảm thiểu triệt để tình trạng AI tạo sinh bị ảo giác (Hallucinations) đối với các Edge cases thông qua các phương pháp thiết kế Prompt (Prompt Engineering) tinh vi.
- Chủ động đề xuất và xây dựng **AI Fallback logic**: ưu tiên dùng luồng OCR Local cho hóa đơn tiêu chuẩn, và trỏ các hóa đơn mờ nát/phi cấu trúc sang Gemini, giảm thiểu hoàn toàn tỷ lệ fail hệ thống.

### Tự Đánh Giá (Self-Assessment)

Để phản ánh một cách khách quan quá trình thực tập, tôi xin tự đánh giá bản thân dựa trên các tiêu chí dưới đây:

| STT | Tiêu chí | Đánh giá | Nhận xét |
|---|---|---|---|
| 1 | Kiến thức chuyên môn | ✅ Tốt | Nắm vững cách tích hợp các model CV/NLP tiên tiến (LayoutLMv3, PaddleOCR, Gemini API) và đóng gói dịch vụ AI trên AWS. |
| 2 | Khả năng học hỏi | ✅ Tốt | Nắm bắt nhanh kỹ thuật Prompting cho GenAI, làm chủ việc huấn luyện LayoutLMv3 phục vụ bài toán hóa đơn Việt Nam phức tạp. |
| 3 | Chủ động | ✅ Tốt | Chủ động đề xuất luồng AI Fallback đa tầng giúp cân bằng tuyệt vời giữa chi phí vận hành và độ chính xác tuyệt đối. |
| 4 | Kỷ luật | ✅ Khá | Tuân thủ nghiêm ngặt tiến độ dự án, liên tục đồng bộ tích hợp với team Backend và duy trì đầy đủ worklog hàng tuần. |
| 5 | Giao tiếp | ✅ Khá | Trình bày rõ ràng các logic kiến trúc AI cho thành viên non-tech, trao đổi hiệu quả hợp đồng JSON payload với team Backend. |
| 6 | Hợp tác nhóm | ✅ Tốt | Phối hợp nhịp nhàng với đội Backend, Frontend và Cloud để luồng xử lý AI đồng bộ hoàn hảo vào hệ thống SmartInvoice Shield. |
| 7 | Giải quyết vấn đề | ✅ Tốt | Khắc phục hiệu quả các điểm thắt nút về độ trễ OCR, xử lý ảo giác từ LLM và xây dựng Rule Engine hậu xử lý cực kỳ cứng cáp. |
| 8 | Đóng góp dự án | ✅ Tốt | Đóng góp thành công động cơ lõi AI OCR với độ chuẩn xác cao, trở thành bộ não định hình trí tuệ cho toàn hệ thống. |

### Cần Cải Thiện (Needs Improvement)
- Cần tính kỷ luật chặt chẽ hơn trong việc cập nhật tài liệu kỹ thuật và độ đo (metrics) ngay lập tức sau mỗi lần cấu hình/tinh chỉnh mô hình nhỏ.
- Cải thiện kỹ năng thuyết trình để thiết kế mô tả các luồng AI học máy phức tạp trở nên trực quan và dễ hiểu hơn, minh bạch hóa luồng xử lý.
- Tiếp tục nghiên cứu sâu thêm các kỹ thuật nén mô hình tĩnh (ví dụ: ONNX Quantization) nhằm hạ sâu ngưỡng độ trễ (Latency) phục vụ tốc độ realtime.