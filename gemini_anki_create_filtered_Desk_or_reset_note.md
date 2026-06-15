Để giải quyết vấn đề này nhanh nhất khi **ngày mai đã thi rồi**, bạn có 2 cách tùy thuộc vào cách bạn muốn học:

- **Cách 1 (Khuyên dùng cho việc thi gấp):** Tạo một bộ bài lọc (Filtered Deck) để gom riêng các thẻ có tag `permissions` ra học cấp tốc ngay lập tức, **không làm ảnh hưởng đến tiến độ/thống kê gốc** của các thẻ này trong Deck Linux.
- **Cách 2:** Đặt lại trạng thái (Reset) toàn bộ các thẻ có tag này về trạng thái "Thẻ mới" (New) để học lại từ đầu như một thẻ mới tinh.

Dưới đây là hướng dẫn chi tiết từng cách trên Máy tính (Anki Desktop):

## Cách 1: Tạo Filtered Deck để ôn cấp tốc (Tốt nhất cho việc đi thi)

Cách này giống như bạn rút các thẻ có tag `permissions` ra một chiếc hộp riêng để cày cuốc đêm nay, thi xong chúng sẽ tự động trả về hộp cũ.

1. Tại màn hình chính của Anki, nhấn phím **`F`** (hoặc vào menu **Tools** -> **Create Filtered Deck...**).
2. Thiết lập các thông số như sau:
- **Name:** `Ôn thi Permissions` (hoặc tên bất kỳ bạn muốn).
- **Search limit:** Nhập vào: `deck:"Linux" tag:permissions`*(Nếu muốn học cả các thẻ đã thuộc lẫn chưa thuộc, bạn cứ để nguyên dòng này).*
- **Limit to:** Chọn số lượng thẻ muốn học (ví dụ: `9999` để lấy hết sạch thẻ).
- **Order:** Chọn **`Random`** (Ngẫu nhiên) hoặc **`Most lapses`** (Những thẻ bạn hay quên nhất).
- **Reschedule cards based on my answers trong cái deck này:** * **BỎ TÍCH (Không chọn):** Nếu bạn chỉ muốn ôn tập để ngày mai đi thi, không muốn câu trả lời hôm nay làm xáo trộn thuật toán Anki sau này.
- **TÍCH CHỌN:** Nếu bạn muốn câu trả lời hôm nay tính vào lịch sử lặp lại (Anki sẽ tự tính toán lại xem khi nào cần nhắc lại dựa trên việc hôm nay bạn nhớ hay quên).
3. Nhấn **Build**.

Bây giờ bạn sẽ thấy một Deck màu xanh dương xuất hiện. Hãy bấm vào đó và "gặm nhấm" hết đống thẻ đó cho kỳ thi ngày mai. Thi xong, bạn chỉ cần bấm vào bánh răng cạnh Deck đó -> chọn **Delete** là xong (yên tâm, thẻ không bị mất, nó chỉ trả về deck Linux cũ).

## Cách 2: Reset toàn bộ thẻ về trạng thái "Thẻ mới" (Học lại hoàn toàn)

Nếu bạn muốn xóa sạch lịch sử và coi như chưa từng học qua các thẻ thuộc tag này:

1. Bấm vào **Browse** (hoặc nhấn phím **`B`**).
2. Ở thanh tìm kiếm phía trên, nhập: `deck:"Linux" tag:permissions` rồi ấn Enter.
3. Nhấp chọn 1 thẻ bất kỳ trong danh sách, sau đó nhấn **`Ctrl + A`** để chọn tất cả các thẻ đang hiển thị.
4. Nhấp chuột phải (hoặc vào menu **Cards** ở phía trên cùng) -> chọn **Forget** (Đặt lại trạng thái).
5. Một hộp thoại hiện ra hỏi bạn có muốn reset vị trí (Queue) không, bạn cứ để mặc định và nhấn **OK**.

> ⚠️ **Lưu ý:** Sau khi làm cách này, toàn bộ các thẻ đó sẽ chuyển thành màu xanh lá cây/xanh dương nhạt (thẻ New) và xếp hàng chờ bạn học. Tuy nhiên, nếu số lượng thẻ quá lớn và giới hạn học thẻ mới mỗi ngày (**New cards/day**) trong cấu hình Deck Linux của bạn quá thấp (ví dụ chỉ 20 thẻ/ngày), bạn sẽ không thể học hết ngay trong hôm nay được. Bạn cần vào Option của Deck Linux để tăng tạm thời `New cards/day` lên tối đa thì ngày mai mới kịp thi.
>
>

Chúc bạn "cày" kịp đêm nay và đạt kết quả tốt vào ngày mai! Bạn có gặp khó khăn ở bước tìm kiếm hay thiết lập filter không?