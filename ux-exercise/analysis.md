## Sản phẩm: MoMo — Moni AI Assistant (trợ lý tài chính)

## 4 paths

### 1. AI đúng
- User hỏi thông tin chi tiêu hoặc giao dịch → Moni trả kết quả đúng
- Hiển thị dữ liệu rõ ràng (số tiền, danh mục, thời gian)
- UI: có summary + icon + context rõ ràng, không cần user chỉnh sửa
- User tin tưởng và tiếp tục sử dụng AI

---

### 2. AI không chắc
- User nhập query mơ hồ hoặc thiếu thông tin
- Moni không trả lời ngay mà yêu cầu thêm dữ liệu (ví dụ: “Bạn muốn xem theo tháng hay tuần?”)
- Có gợi ý prompt để user chọn nhanh
- Vấn đề: tăng thêm bước tương tác → có thể gây friction nhẹ

---

### 3. AI sai
- Moni hiểu sai ngữ cảnh hoặc đưa ra thông tin không chính xác
- User phát hiện lỗi trong nội dung phản hồi
- Sửa: phải chat lại, cung cấp lại thông tin → nhiều bước (3–4 bước)
- Vấn đề:
  - Không có cách sửa trực tiếp (inline)
  - Flow phụ thuộc hoàn toàn vào chat → dễ lặp và hiểu sai
  - Không rõ AI có học từ correction hay không

---

### 4. User mất niềm tin
- Sau nhiều lần AI trả sai → user không còn tin vào kết quả
- User chuyển sang:
  - Bỏ qua AI
  - Thao tác thủ công
- Vấn đề:
  - Không có cơ chế fallback rõ ràng
  - Không tách biệt AI vs manual
  - Không có option kiểm soát (ví dụ: ưu tiên manual)

---

## Path yếu nhất: Path 3 + 4
- Khi AI sai, recovery flow quá dài và phức tạp
- Không có feedback loop rõ (user sửa nhưng không biết AI có học không)
- Không có cơ chế khôi phục niềm tin (trust recovery)
- Thiếu exit/fallback rõ ràng khi user không muốn dùng AI

---

## Gap marketing vs thực tế
- Marketing: “AI giúp quản lý tài chính thông minh, cá nhân hóa”
- Thực tế:
  - AI hoạt động tốt với case đơn giản
  - Các trường hợp phức tạp (thiếu context, nhiều ý định) dễ sai
- Gap lớn:
  - Marketing không đề cập đến error handling
  - User kỳ vọng AI chính xác cao → dễ thất vọng khi sai

---