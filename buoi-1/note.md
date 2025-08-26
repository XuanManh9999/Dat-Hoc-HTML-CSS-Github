# Giới thiệu HTML là gì, các thẻ thông dụng h1..h6, p, span, div, table, select option, form, label, a, button các thuộc tính phổ biến

HTML là một ngôn ngữ đánh dấu siêu văn bản. Nó không phải ngôn ngữ lập trình, HTML là ngôn ngữ kịch bản.
Nhiệm vụ của nó trong website là đánh dấu các chữ, hình ảnh, bố cục, video....

Cú pháp thẻ html
+,  <tag></tag> gồm cả thẻ mở và thẻ đóng
+, <img/> thẻ bao gôm cả thẻ mở và thẻ đóng

# Các thẻ thông dụng trong html
+, Thẻ về tiêu đề: h1-h6. Lưu ý là một trang  không nên để các tiêu đề bị trùng lặp tứ là phải có thứ tự từ bé đến lớn

+, Thẻ văn bản: p(văn bản dài), span (văn bản ngắn)
+, Thẻ hình ảnh: img thằng này nó gồm 2 thuộc tính src="nguồn hình ảnh", alt="mô tả hình ảnh, khi ảnh bị lỗi sẽ kích hoạt nột dung"
+, Các loại thẻ danh sách: ul(danh sách không có thứ tự), ol (danh sách có thứ tự), li (các phần tử trong danh sách đó)

Các loại thẻ input: thẻ input có nhiều type: 
+, text(nội dung thường, mặc định)
+, password hiển thị dạng * thay vì tường minh mật khẩu
+, radio dạng check radio (chỉ cho phép chọn 1)
+, checkbox dạng check box (cho phép chọn nhiều)
+, range khoảng (cho phép chọn khoảng giá trị)
+, date hiển thị này tháng
+, number chỉ cho phép dạng số

+, Thẻ ngắt lề: br (dùng khi muốn ngắt dòng. Tức là nội dung sau nó sẽ xuống một dòng mới)

+, Thẻ tạo bảng: table, tr(dòng), td (dữ liệu dòng), th(tiêu đề hàng)
- colspan: quy định chiếm bao nhiêu cột
- rowspan: quy định chiếm bao nhiêu dòng

+, Thẻ lựa chọn: select, option thẻ này dùng dể người dùng có thể chọn 1 hoặc nhiều kết quả


+, Thẻ form(label, input, buton..) dùng khi có nhu cầu submit dữ liệu lên phía server. Và thẻ này có 2 thuộc tính cần nhớ là:
- action: địa chỉ submit
- method: phương thức http submit GET (default), POST
- target: giống thẻ a


+, Thẻ a. Thẻ a dùng để liên kết, hoặc chuyển hướng đến một cài nguyên theo đường dẫn
- href: đường dẫn
- target: _self, blank

+, button: Nút. Trong ngữ cảnh form thì thẻ button là dùng để submit (mặc đinh) nó gồm một số type:
- button -> là 1 nút bình thường
- submit -> submit form 
- reset -> thì nó sẽ reset mọi nội dung trong trang