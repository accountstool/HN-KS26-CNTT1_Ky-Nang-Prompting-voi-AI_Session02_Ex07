
## Phần 1. Thiết kế 6 khối CREATE

- Character: giao vai trưởng nhóm CSKH dày dạn xử lý khủng hoảng của TechShop, để AI viết dưới danh nghĩa chịu trách nhiệm thay vì một trợ lý nằm ngoài cuộc
- Request: nhiệm vụ cụ thể là email xin lỗi khách hàng về đơn linh kiện PC chậm 4 đến 6 ngày, có nhận lỗi, giải trình, cam kết giao lại và ưu đãi bồi thường
- Examples: câu văn mẫu thể hiện đồng cảm để AI bắt chước độ chân thành, tránh kiểu xin lỗi máy móc
- Adjustment: các điều cấm kỵ theo đúng ràng buộc của đề, không đổ lỗi đơn vị vận chuyển, không hứa suông thiếu mốc thời gian, không chữ ký sáo rỗng
- Type of Output: khung email chuẩn với tiêu đề, lời chào trang trọng, 3 đoạn thân bài, lời cam kết và thông tin liên hệ khẩn cấp
- Extras: voucher giảm 15% cho đơn sau và hotline VIP, hai "gia vị" bồi thường đề bắt buộc phải có

## Phần 2. Master Prompt hoàn chỉnh

```text
[C] Character: Bạn là Trưởng nhóm Chăm sóc Khách hàng của TechShop, người chịu trách nhiệm chính xử lý khủng hoảng giao hàng đợt Black Friday này
[R] Request: Soạn email xin lỗi gửi đích danh khách hàng [tên khách] về đơn linh kiện PC gồm card màn hình, Nguồn, RAM bị giao chậm 4 đến 6 ngày so với cam kết, trong đó nhận lỗi trực tiếp, giải trình nguyên nhân, cam kết lộ trình giao hàng mới và ưu đãi bồi thường
[E] Examples: Câu mẫu để bắt chước mức đồng cảm: "Chúng tôi hiểu anh/chị chờ đợi không chỉ một đơn hàng, mà là kế hoạch nâng cấp máy mình chăm chút từ lâu, và chúng tôi thật sự có lỗi vì làm gián đoạn kế hoạch đó"
[A] Adjustment: Không đổ lỗi cho đơn vị vận chuyển hay bất kỳ bên nào, không hứa suông thiếu mốc thời gian cụ thể, không dùng chữ sáo rỗng kiểu "rất tiếc về sự bất tiện", giữ giọng cầu thị, chuyên nghiệp, đồng cảm từ đầu tới cuối
[T] Type of Output: Email chuẩn gồm tiêu đề rõ ràng, lời chào trang trọng, 3 đoạn thân bài súc tích theo thứ tự nhận lỗi, giải trình minh bạch nguyên nhân kho phân loại tự động quá tải, lộ trình giao hàng mới kèm mốc cụ thể, kết thúc bằng lời cam kết và thông tin liên hệ khẩn cấp
[E] Extras: Cuối email tặng voucher giảm 15% cho đơn hàng sau với mã [voucher], ghi rõ hotline [hotline] hỗ trợ 24/7 cho khách bị ảnh hưởng, ký tên Bộ phận Chăm sóc Khách hàng TechShop
```
