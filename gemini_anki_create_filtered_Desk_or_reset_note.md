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
---
Đoạn văn trên trích từ tài liệu hướng dẫn của Anki, giải thích về tính năng **Custom Study (Học tùy chỉnh)**. Đây là cách nhanh nhất và tiện nhất để bạn tạo ra một bộ bài lọc (Filtered Deck) thông qua các thiết lập có sẵn (presets) mà không cần phải tự gõ các câu lệnh tìm kiếm phức tạp.

Dưới đây là bản dịch và giải thích chi tiết, dễ hiểu cho từng phần:

## 1. Khái niệm chung về Custom Study

> *Cách dễ nhất để tạo một bộ bài lọc (filtered deck) là sử dụng nút **Custom Study**, nút này xuất hiện ở dưới cùng màn hình khi bạn bấm chọn một Deck nào đó. Nó cung cấp các bộ lọc có sẵn rất tiện lợi cho các tác vụ phổ biến, chẳng hạn như ôn lại các thẻ bạn đã bấm trượt (nhấn nút Again) trong ngày hôm đó. Nó sẽ tạo ra một deck lọc tên là **"Custom Study Session"** và tự động mở ra cho bạn học.*
>
> *Nếu một deck tên "Custom Study Session" đã tồn tại từ trước, nó sẽ bị xóa sạch thẻ bên trong trước khi nạp các thẻ mới vào. Nếu bạn muốn giữ lại deck tùy chỉnh này để học lâu dài, bạn chỉ cần đổi tên (Rename) nó ở danh sách Deck ngoài màn hình chính.*
>
>

## 2. Giải thích chi tiết các tùy chọn (Options)

Khi bạn bấm vào **Custom Study**, Anki sẽ cho bạn các lựa chọn sau:

### 📈 Tăng giới hạn thẻ trong ngày (Không tạo deck mới)

- **Increase today’s new card limit (Tăng giới hạn thẻ mới hôm nay):** Thêm thẻ mới vào ngay deck bạn đang học.
- *Lưu ý:* Khác với các tùy chọn bên dưới, tính năng này **không** tạo ra deck lọc mới, mà nó trực tiếp sửa đổi (tăng tạm thời) giới hạn của deck hiện tại.
- **Increase today’s review card limit (Tăng giới hạn thẻ ôn tập hôm nay):** Nếu số thẻ đến hạn (due) hôm nay quá nhiều và bị nghẽn lại do giới hạn hàng ngày (Daily review limit) bạn cài đặt trước đó, tùy chọn này cho phép bạn "mở khóa" để xem thêm các thẻ bị nghẽn đó. Tương tự như thẻ mới, nó sửa đổi trực tiếp trên deck hiện tại chứ không tạo deck mới.

### 🧠 Ôn tập chuyên sâu (Tạo deck lọc "Custom Study Session")

- **Review forgotten cards (Ôn lại các thẻ bị quên):** Gom lại và hiển thị tất cả các thẻ mà bạn đã lỡ bấm **Again (Số 1)** trong vòng số ngày mà bạn chỉ định (ví dụ: gom các thẻ bị bấm trượt trong vòng 3 ngày qua để học lại).
- **Review ahead (Học trước thời hạn):** Học trước những thẻ sắp đến hạn trong tương lai gần (theo số ngày bạn chỉ định).
- *Mẹo nhỏ:* Cách này cực kỳ hữu ích để bạn "cày trước" bài vở trước khi đi du lịch hoặc nghỉ lễ. Tuy nhiên, nó sẽ không có tác dụng nhiều với các thẻ bạn vừa mới học xong.
- **Preview new cards (Xem trước thẻ mới):** Xem qua các thẻ bạn vừa mới thêm vào gần đây, nhưng **không** kích hoạt thuật toán học (tức là bạn bấm trả lời xong thì trạng thái của thẻ vẫn giữ nguyên là thẻ mới tinh, không bị chuyển thành thẻ đang học).
- **Study by card state or tag (Học theo trạng thái thẻ hoặc theo Tag):** **(Chính là tính năng bạn đang cần cho kỳ thi ngày mai!)**
- Nó cho phép bạn bốc một số lượng thẻ nhất định từ deck hiện tại ra để học.
- Bạn có thể chọn: chỉ lấy thẻ mới (New), chỉ lấy thẻ đến hạn (Due), hoặc lấy tất cả các thẻ (All).
- Sau khi bấm nút **"Choose Tags"**, bạn có thể tích chọn riêng tag `permissions` để học.
- *Lời khuyên từ tài liệu:* Nếu bạn muốn gom **tất cả sạch sành sanh** các thẻ trong tag đó ra học (ví dụ để ôn thi trước một kỳ thi lớn), hãy điền số lượng thẻ cần lấy lớn hơn tổng số thẻ bạn đang có trong deck (ví dụ điền hẳn `9999`).
Chúc bạn "cày" kịp đêm nay và đạt kết quả tốt vào ngày mai! Bạn có gặp khó khăn ở bước tìm kiếm hay thiết lập filter không?
---
Đoạn tài liệu này hướng dẫn cách **Tự tạo Bộ bài lọc bằng tay (Manually)** dành cho người dùng nâng cao và giải thích chi tiết ý nghĩa của các **Chế độ sắp xếp thứ tự thẻ (Order)**.

Dưới đây là phần giải thích ngắn gọn, đi thẳng vào trọng tâm để bạn nắm bắt ngay lập tức:

## 1. Tạo Filtered Deck bằng tay (Creating Manually)

- **Tự do tùy biến:** Thay vì dùng các mẫu có sẵn của *Custom Study*, bạn vào **Tools -> Create Filtered Deck** để tự gõ lệnh tìm kiếm (ví dụ: `tag:permissions`). Bạn có thể dùng mọi lệnh tìm kiếm giống như trong cửa sổ Browse.
- **Cơ chế hoạt động:** Khi bạn bấm **Build**, Anki sẽ **tạm thời** bốc các thẻ thỏa mãn điều kiện từ deck gốc bỏ vào deck lọc này.
- **Nút Rebuild (Làm mới):** Nếu ngày nào bạn cũng muốn gom thẻ theo điều kiện đó để học (ví dụ: gom thẻ tag `permissions` để kiểm tra bài cũ mỗi sáng), bạn chỉ cần bấm **Rebuild** ở dưới đáy màn hình của Deck đó để Anki tự quét và gom thẻ mới vào lại.
- **Ngoại lệ:** Deck lọc **KHÔNG THỂ** hút các thẻ đang bị **Hoãn (Suspended)**, **Ẩn tạm thời (Buried)**, hoặc các thẻ **đang nằm ở một Deck lọc khác**. Đó là lý do vì sao đôi khi bạn tìm trong Browser thấy có thẻ, nhưng khi Build deck lọc thì thẻ không nhảy vào.
- **Limit & Second Filter:** * *Limit:* Giới hạn số lượng thẻ được hút vào.
- *Enable second filter:* Cho phép bạn gom thẻ bằng 2 điều kiện tìm kiếm song song (Ví dụ: Nhánh 1 gom 50 thẻ cũ đến hạn học trước, Nhánh 2 gom thêm 10 thẻ mới tinh học sau).

## 2. Ý nghĩa các chế độ sắp xếp (Order)

Khi số lượng thẻ thỏa mãn điều kiện **lớn hơn** giới hạn (Limit) bạn đặt ra, Anki sẽ ưu tiên bốc các thẻ theo thứ tự bạn chọn dưới đây và bỏ qua các thẻ ở cuối danh sách:

- **Oldest seen first:** Ưu tiên những thẻ đã lâu lắm rồi bạn chưa ôn lại.
- **Random:** Xáo trộn ngẫu nhiên toàn bộ thẻ (Không theo quy luật nào).
- **Increasing intervals:** Ưu tiên thẻ có khoảng cách lặp lại (interval) **ngắn nhất** trước (thường là thẻ khó, thẻ mới học).
- **Decreasing intervals:** Ưu tiên thẻ có khoảng cách lặp lại **dài nhất** trước (thẻ bạn đã nhớ rất sâu).
- **Most lapses:** Ưu tiên những thẻ bạn **bị bấm sai (Again) nhiều lần nhất** (Cực tốt để trị các thẻ "lỳ lợm" hay quên trước khi đi thi).
- **Order added:** Thẻ nào tạo trước học trước (theo ngày tạo).
- **Latest added first:** Thẻ nào mới tạo gần đây học trước (ngược với cái trên).
- **Order due:** Thẻ nào đến hạn trước thì học trước.
- **Relative overdueness (Độ quá hạn tương đối - Rất thông minh):** Ưu tiên hiển thị những thẻ mà **khả năng cao là bạn đã quên** dựa trên thuật toán.
- *Nếu dùng thuật toán cũ (SM-2):* So sánh tỷ lệ ngày quá hạn / khoảng cách lặp. Ví dụ: Thẻ 5 ngày mà trễ mất 2 ngày (trễ 40%) sẽ được học trước thẻ 10 ngày mà trễ 3 ngày (trễ 30%).
- *Nếu dùng thuật toán mới (FSRS):* Tính toán dựa trên **Khả năng gợi nhớ (Retrievability)** thực tế của từng thẻ kết hợp với mục tiêu duy trì trí nhớ (Desired Retention) bạn cài đặt. Thẻ nào có phần trăm nhớ tụt sâu nhất sẽ hiện lên đầu tiên.

