# Học về lớp giả (:), phần tử giả (::) của CSS
+, Lớp giả
:hover -> áp dụng khi cho chuột vào phần tử
:active -> áp dụng khi click chuột
:focus -> áp dụng khi ta focus vào (nó chỉ tồn tại trong các thẻ form) nếu muốn tạo focus cho các thẻ không năm trong form thì ta dùng thuộc tính (tabindex) 
:checked -> nó thể hiện trạng thái check của check box, radio
:disabled -> dùng khi muốn thay đổi style mặc định của input là disabled
:not() -> nội dung trong not là 1 selector
:first-child: thành phần con đầu tiên
:last-child: thành phần con cuối cùng
:first-of-type: thành phần con đầu tiên và đúng kiểu mới áp dụng
:last-of-type: thành phần con cuối cùng đúng kiểu mới áp dụng
:nth-child(number) chọn phần tử con thứ n
:nth-of-type(number) chọn phần tử con thứ n nhưng phải đúng kiểu mới áp dụng
2n + 1 -> lẻ áp dụng  (n = 0)
2n ->  chẵn (n = 0)


+, phần tử giả
::before: thêm nội dung vào đằng trước của thẻ -> bắt buộc phải thuôc tính content
::after: thêm nội dung vào đằng sau của thẻ -> bắt buộc phải thuôc tính content
::first-line: dòng đầu tiên của chữ sẽ được tác động
::first-letter: chữ cái cầu tiên sẽ bị tác động
::section: khi ta select lên các element
::placeholder đổi màu thuộc tiinhs placeholder của input


# Học về tính kế thừa trong css
Trong CSS thì nó có 2 thuộc tính quyết định việc kế thừa:
+, Initial: kế thừa mặc định của trình duyệt (font-size: 16px;) // user agent stylesheet
+, Inherit: kế thừa từ thằng cha (có đệ quy)



# Flexbox là một mô hình bố cục  1 chiều, giúp sắp xếp, căn chỉnh hoặc giãn/thu linh hoạt 
# theo 2 trục main axis (trục chính), trục chéo (cross axits)

# Để kích hoạt được flex box thì ta cần 1 thằng cha

# Container (cha)
- display: flex | inline-flex; -> biến phần tử thành flex-container
- flex-direction: row | row-reverse | column | column-reverse -> quyết định hướng trục chính
- flex-wrap: nowrap | wrap | wrap-reverse -> cho phép item có xuống hàng hay không
- flex-flow: direction  wrap; -> thuộc tính viết tắt của flex-direction-flex-wrap
- justify-content: flex-start, flex-end, center, space-between (sát lề trái, phải, khoảng cách giữa các phần từ là giống nhau), space-around, space-evenly (khoảng cách đều) (căn theo trục chính)
- align-item: stretch, flex-start,  flex-end, center, baseline(căn theo trục chéo )
- gap: row-gap, column-gap px(đơn vị); tạo khoảng cách thật giữa các item

- align-content: stretch, flex-start,  flex-end, center, space-between, space-around, space-evenly (chỉ tác động khi có nhiều dòng wrap)

# Mẹo nhớ
Nằm ngang (row): justify = trái/phải; align = trên/dưới
nằm dọc (column): justify = trên/dưới; align = trái/phải

# Item (con)
- flex-grow: number -> giãn theo phần free space
- flex-shrink: number ->  thu nhỏ khi thiếu chỗ
- flex-basic: length | auto -> kich thước cơ sở trên trục chính
- flex: grow shrink basis; viết tắt
- align-self: auto | flex-end | center; ghi đè align-item
- margin-left: auto; trick đẩy item sang cuối trục
- order: number -> Sắp xếp flex-item theo thứ tự