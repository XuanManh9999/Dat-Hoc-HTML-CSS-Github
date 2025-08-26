Học về khái niệm thẻ inline, block, inline-block. id, class khi nào dùng, Semantic(HTML 5), mở đầu về css giới thiệu 3
dạng internal, extenal, inline, học về css selector, Pseudo Elements
Pseudo Classes, Các đơn vị thường dùng trong CSS

# Tất cả các thẻ html đều có một trong 2 thuộc tính này
+, display: inline; -> Các phần tử sẽ có chiều rộng bằng với chiều rộng nội dung của chính nó (span, strong...). Cho nên các nội dung có thể nằm cùng một hàng (không cho set kích thướng)
+, display: block; -> Mặc định phần tử nó sẽ chiếm hết chiều rộng màn hình của nó. Và chính vì thế nên các nội dung đứng sau nó thì sẽ bắt đầu trên một hàng mới (div, h1...)
+, display: inline-block; -> Cũng tương tự như inline nhưng nó cho phép ta set kích thướng

# Học về ID (#) và class(.)
+, ID: mỗi một thẻ chỉ có thể có 1 id và id thì không được phép trùng nhau trong trang web.
+, class: khác với id nó có thể trùng nhau, và dùng thoả mái, tái sử dụng được


# Semantic(HTML5) -> ngữ nghĩa của thẻ html, mục đích là giúp con bot của google hiểu nội dung website của mình truyền tải nội dung gì, và từ đó tăng thứ hạng tìm kiếm

# Các thẻ Semantic(HTML5) thông dụng:
+, <header></header> được sử dụng cho phần đầu trang web. hoặc các phần tử đầu của các thẻ
+, <nav></nav> được sử dụng cho phần navigator(phần điều trang)
+, <section></section> được sử dụng để tạo thành một khu vực bao gồm những nội dung giống nhau
VD: khu vực sản phẩm, khi vực bài viết, khu vực tin tức
+ <article></article> được sử dụng cho các phần có ý nghĩa riêng biệt và độc lập với các thành phần còn lại VD: Bài viết, sản phẩm, bình luận
+, <aside></aside> được sử dụng để chứa những thông tin bên cạnh nội dung chính
+, <footer></footer> được sử dụng cho phần cuối của trang hoặc phần cuối của một thẻ
+, <main></main> chứa thân của trang web
+, <figure></figure>, <figcaption></figcaption> thẻ hiện đối đượng cần tách biệt VD hình ảnh, biểu đồ

+, <strong></strong> nó dúng để nhấn mạnh những nội dung quan trong (inline). VD: Địa danh, tên tác giả

# CSS là một ngôn ngữ được sử dụng để định dạng các trang web. Nó xác định các các phần tử HTML được hiển thị trên màn hình, bao gồm: màu sắc, kích thước, bố cục... Giúp tạo ra giao diện trực quan cho người dùng
Có 3 kiểu CSS:
+, External: tạo ra một file css rồi dùng thẻ link để liên kết tới. (hay dùng) +
+, Internal: css ở trên phần thẻ head và dùng cặp thẻ <style></style> ít sử dụng vì làm dài file code. +
+, Inline: css thẳng vào bằng thuộc tính style của thẻ html (ít dùng làm dài code) +++

# Học về css Selector
# Css selector nó chỉ đơn giản là cách mà ta chọn các phần tử html để css cho chúng
+, * -> áp dụng cho tất cả các thẻ
+, tên thẻ: dùng chính tên thẻ html để css. VD: h1 {color: red}
+, dùng giá trị class. VD: <h1 class="h1 h2"></h1> => selector => .h1 {color: red}
+, dùng giá trị id. VD: <h1 id="h1"></h1> => selector => #h1 {color: red}
+, tag1 tag2: chọn thẻ tag_2 nằm trong tag_1
+, tag1 > tag2: chọn thẻ tag_2 là con trực tiếp của tag1
+, .tag1.tag2: chọn element chứa cả 2 class là tag1 và tag2
+, tag1 ~ tag2: chọn những phần tử nằm sau tag1 với tag2 là ngang hàng với tag1
+, tag1 + tag2: chọn tag2   nó nằm ngay sau tag1
+, tên tag[thuộc tính=giá trị] {

} -> selector dựa trên giá trị thuộc tính



