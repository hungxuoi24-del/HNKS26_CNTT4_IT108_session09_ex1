
# BÀI TẬP 1: CHUẨN HÓA TÀI LIỆU MARKDOWN CHO DỰ ÁN

## Phần 1. Phân tích lỗi cú pháp

Dựa trên đoạn mã gốc của bạn sinh viên, hệ thống render bị lỗi và lộn xộn do các nguyên nhân sau:

1. **Lỗi nhảy cóc cấp độ Heading (H1 xuống H3):** 
   - Đoạn mã sử dụng `# Lợi ích của rau sạch` (H1) nhưng ngay dòng sau lại dùng `### Danh sách các loại rau` (H3), bỏ qua cấp `##` (H2). Điều này làm đứt gãy cấu trúc phân cấp tài liệu ngữ nghĩa (semantic hierarchy).
2. **Lỗi cú pháp chèn hình ảnh (Image syntax):** 
   - Dòng `[Logo Dự án] ( https://greentech.vn/logo.png )` bị khoảng trắng thừa giữa cặp ngoặc vuông `[...]` và ngoặc tròn `(...)`. Trong chuẩn Markdown, cú pháp ảnh bắt buộc phải có dấu chấm than ở đầu (`!`) và viết liền mạch không chứa khoảng trắng giữa hai khối ngoặc `![Alt Text](URL)`.
3. **Lỗi định dạng in đậm (Emphasis syntax):** 
   - Đoạn văn bản `*Rất quan trọng (chỉ dùng 1 dấu sao thay vì 2 để in đậm)*` chỉ sử dụng một dấu sao (`*`), khiến trình soạn thảo nhận diện nhầm thành chữ nghiêng (Italic) thay vì chữ in đậm (Bold, yêu cầu phải dùng `**`).

---

## Phần 2. Đoạn mã hoàn thiện (Copy dán trực tiếp vào StackEdit)

# Lợi ích của rau sạch

## Danh sách các loại rau

![Logo Dự án](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQCMspAV052nOJ3AwGlmjCT_vywVrWweDt8ycQlV4VjaA&s=10)

**Rất quan trọng**

