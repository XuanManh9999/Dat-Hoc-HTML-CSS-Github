# Position là gì?

positon trong css dùng để xác định cách một phần tử được đặt trong layout của trang web. Nó quyết định phần tử đó sẽ đứng ở đâu và có thể di chuyển theo các hướng. top, left, right, buttom như thế nào

# Các giá trị của positon

+, static(mặc định): tất cả các phần tử HTML mặc định đều có, nó không chịu ảnh hưởng của
top, left, right, buttom. Phần tử sẽ nằm trong luồng bình thường của trang

+, relative: phần tử nó vẫn nằm trong bố cục luồng, nhưng có thể dịch chuyển nó so với chính vị trị của nó ban đầu bằng các thuộc tính. top, left, right, bottom. Khoảng trống ban đầu vẫn được dữ lại

+, absolute: phần tử lúc này sẽ bị loại bọ bố cục luồng bình thường, nó được đặt tương đối với phần tử gần nhất có thuộc tính positon khác static. Nếu không có thằng cha nào có position, nó sẽ bám theo thẻ html

+, fixed: giống absolute, nhưng nó luôn cố định theo hướng cửa sổ trình duyệt (viewport), không phụ thuộc vào phần tử cha. Thường dùng để tạo menu cố định, nút scroll lên đầu trang

+, sticky: Là sự kết hợp của relative và fixed.
Ban đầu, phần tử hoạt động như relative, khi cuộn trang đến ngưỡng
VD (top: 0), nó chuyển sang hoạt động như fixed cho đến khi phần tử cha kết thúc
// dời khỏi bố cục luồng thì sẽ không bị va đập

# Học về animation

+, transform: biến đổi khung vẽ của phần tử (xoay, tịnh tiến, phóng to, thủ nhỏ...) mà không làm thay đổi layout (không chiếm diện tích chỗ khác)
+, phần trăm trong transform là theo kích thước của chính phần tử đó, không phải theo phần tử cha

# Các thuộc tính của transform:

# Các hàm 2D

+, translate(x, y), translateX, translateY -> tịnh tiến
+, scale(x, y) / scaleX(), scaleY() -> phóng thu (mặc định là 1 tương đương 100%)
+, rotate(angle) độ VD: 360deg -> xoay trục z
+, skew(x, y) / skewX, skewY -> nghiêng

# Các hàm 3D:

+, translateZ, scaleZ, rotateX, rotateY, rotateZ

# Transition

- transition giúp phần tử chuyển đổi mượt mà từ trạng thái này sang trại thái khác khi có thay đổi CSS (hover, focus, active)
- nếu không có transition sự thay đổi nó sẽ xảy ra ngay lật tức

# Cú pháp đầy đủ:

transition: thuộc tính css (all, width, opactity, transform) | thời gian chuyển động (ms, s) | animation (ease, linner...) | delay

# Các giá trị hay dùng

+, transition-duration (thời gian chuyển động)
Thường dùng ms, s VD 200ms(2s), 0.5s
+, Thời gian chuyển cảnh

- ease (mặc định): mặc định, chậm ở dầu / cuối
- liner: tốc độ đều
- ease-in: chậm đầu, nhanh cuối
- ease-out: nhanh đầu, chậm cuối
- ease-in-out: chậm đầu & cuối, nhanh ở giữa
  +, Delay
- Thời gian chờ trước khi bắt đầu
  VD: 2s -> sau 2 giây thì nó mới bắt hoạt ảnh
