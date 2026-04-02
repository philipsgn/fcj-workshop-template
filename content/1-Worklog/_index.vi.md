---
title: "Nhật ký công việc"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

Dưới đây là nhật ký quá trình 12 tuần thực tập với vai trò AI Developer, tập trung vào việc nghiên cứu, phát triển hệ thống Invoice OCR kết hợp với việc học hỏi và thực hành triển khai các dịch vụ Đám mây cơ bản của nền tảng AWS.

Quá trình thực tập có thể được chia thành 4 giai đoạn chính (Phases):
1. **Giai đoạn 1 (Tuần 1-4): AWS Foundations & AI Prep.** Xây dựng môi trường lưu trữ, tính toán linh hoạt (EC2, S3, Lambda) và đánh giá các mô hình OCR.
2. **Giai đoạn 2 (Tuần 5-8): Core Model & Cloud Integration.** Huấn luyện mô hình AI cốt lõi, Container hóa lên ECS/ECR và sử dụng luồng RDS, SQS.
3. **Giai đoạn 3 (Tuần 9-11): LLM Integration & Optimization.** Tích hợp LLM, giám sát hiệu năng với CloudWatch và bảo mật hạ tầng.
4. **Giai đoạn 4 (Tuần 12): Resilience & Finalization.** Hoàn thiện kiến trúc Fallback và triển khai tự động lên Production.

**Tuần 1:** [AWS Foundations & Environment. Học về IAM, VPC cơ bản; thiết lập EC2 instance để tạo môi trường tính toán Jupyter/PyTorch.](1.1-week1/)

**Tuần 2:** [Cloud Storage & Baseline OCR. Tìm hiểu Amazon S3 để lưu kho dữ liệu hóa đơn; đánh giá baseline model với Amazon Textract và Tesseract.](1.2-week2/)

**Tuần 3:** [Serverless Compute & Data Pipeline. Ứng dụng AWS Lambda và S3 Event trigger để tự động hóa thuật toán tiền xử lý ảnh (Deskew, Binarize).](1.3-week3/)

**Tuần 4:** [Containerization & Annotation. Đóng gói môi trường (Docker) đẩy tải lên Amazon ECR; thiết lập bộ quy chuẩn Ground Truth và gia tăng dữ liệu (Data Augmentation).](1.4-week4/)

**Tuần 5:** [Model Training & Compute Scaling. Huấn luyện mô hình OCR Layout-aware, tìm hiểu khái niệm các dòng EC2 hỗ trợ GPU/SageMaker để rút ngắn thời gian train.](1.5-week5/)

**Tuần 6:** [API Development & Entity Mapping. Xây dựng logic AI trích xuất thông tin (Tên, MST) và nghiệm thu triển khai kiến trúc Server với Amazon ECS/Fargate.](1.6-week6/)

**Tuần 7:** [Database Storage & Table Extraction. Giải bài toán trích xuất mảng hàng hóa (Line Items) và trực tiếp lưu trữ kết quả JSON vào Database (Amazon RDS/DynamoDB).](1.7-week7/)

**Tuần 8:** [Queue Systems & Model Evaluation. Phối hợp AWS SQS tạo hàng đợi xử lý hóa đơn đồng loạt bất đồng bộ; đánh giá F1-score và tinh chỉnh mô hình AI.](1.8-week8/)

**Tuần 9:** [LLM Integration & Prompt Engineering. Trải nghiệm tích hợp mô hình ngôn ngữ lớn (Gemini/Amazon Bedrock) làm bước xử lý Fallback cho hóa đơn ảo/nhòe nát.](1.9-week9/)

**Tuần 10:** [Performance Tuning & Monitoring. Tối ưu độ nhạy bộ nhớ AI; thiết lập Amazon CloudWatch Dashboard để bám sát các metric từ việc gọi lại API và ghi log báo lỗi.](1.10-week10/)

**Tuần 11:** [Security & Confidence Validation. Xây dựng AI chấm điểm tin cậy, tự động tính chéo (Math Validation); bảo mật API Keys an toàn nhờ AWS Secrets Manager / Parameter Store.](1.11-week11/)

**Tuần 12:** [System Resilience. Tập trung hoàn chỉnh hệ thống dự phòng (AI Fallback), bọc lót Edge Cases và đưa kiến trúc OCR xử lý hóa đơn cuối cùng lên môi trường Production.](1.12-week12/)