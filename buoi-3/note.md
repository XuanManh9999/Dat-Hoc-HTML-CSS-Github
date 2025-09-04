# BEM là gì?
BEM là cách đặt tên class trong html và từ khóa BEM viết tắt của (Block - Element - Modifier)
Syntax:
- Block: block -> thành phần cha đầu tiên, bao bọc
- Element: block__element -> các thành phần con bên trong
- Modifier:  -> Đặc điểm của block
    - Block: block--modifier  
    - Element: block__element--modifier

<div class="container">
    <div class="container__item">
        <div class="container__item__img">
            <img/>
        </div>
        <p class="container__item__desc">bababâ</p>
        <button class="container__item__submit">Submit</button>
    </div>
</div>

# Ưu điểm của BEM
+, Loại bỏ ID và tên thẻ trong css
+, Gần như không xếp trồng
+, Các khối code nó sẽ độc lập với nhau



# Mở đầu về các thuộc tính css

# Thuộc tính CSS

# Thuộc tính về màu sắc:
+, color: value; -> màu chữ
+, background-color: value; -> màu nền
+, background-image: value; -> ảnh nền
+, background-size: value; -> kích thước ảnh nền -> cover (nội dung hài hòa chấp nhận che khuất nội dung đi), contain (không quan tâm kích thước và luôn đảm bảo hình ảnh nền được hiển thị đầy đủ)
+, background-repeat: value; -> lặp lại ảnh nền; repeat -> lặp lại, no-repeat: không lặp lại
repeat-x -> lặp lại theo trục ngang, repeat-y là trục dọc
+, opacity: value (0-1); -> độ trong suốt

# Thuộc tính về kích thước và khoảng cách
+, width/hight: chiều rộng/chiều cao VD 100px
+, max-width/min-width (tương tự cho hight): chiều rộng tối ta/chiều rộng tối thiệu

+, padding: khoảng cách bên trong element
   /* padding: 10px 20px 30px 50px;  trên, phảo, dưới, trái*/
    /* padding: 20px 50px 100px; trên, phải, trái, dưới*/
    /* padding: 20px 50px; trên dưới, phải trái*/
    /* padding: 20px; all */
+, margin: khoảng cách bên ngoài (kc giữa các phần tử)
    /* margin: 10px;  */
    /* margin: 10px 20px 30px 40px; */
    margin-top: 10px;
    margin-bottom: 10px;
    margin-left: 10px;
    margin-right: 10px;
+, border: Viền
    /* border-width: 5px; */
    /* border-style: dashed; dashed nét đứt, solid nét liền */
    /* border-style: double; */
    /* border-color: gold; */
    /* viết tắt border sẽ gồm: border: kích thước kiểu màu */
+, box-sizing: Cách trình duyệt tính kích thước (border-box là chuẩn nhất)

# Thuộc tính về văn bản text
+, font-size: value; -> cơ chữ
+, font-weight: 100 - 900; -> độ đậm của chữ
+, font-family: tên kiểu; kiểu chữ 
+, text-align: ; Căn lề (theo chiều ngang nội dung) Lưu ý chỉ căng được thẻ có dạng block, và inline-block
    /* text-align: left;  left (default), center, right */
+, text-decoration: tyle; gạch chân, gạch ngang chữ
+, light-height: khoảng cách giữa các dòng
    /* line-height: 3; 1.4 (tiếng anh), tiếng việt là 1.6*/
+, letter-spacing: khoảng cách giữa các chữ
    letter-spacing: 20px;

+, text-transform: quy định cách các phần tử được hiển thị in hết, thường hết
    /* text-transform: uppercase; */
    /* Viết hoa tất cả chữ cái */
    /* text-transform: lowercase; /* Viết thường tất cả chữ cái */

# Các đơn vị trong css thường dùng
+, px: đơn vị đo độ dài tuyệt đối. dựa trên pixel
+, %: đơn vị đo phần trăm của một giá trị so với giá trị gốc (giá trị cha gan nhat)
+, em: đơn vị đo phần trăm của font-size của phần tử cha VD cha 30px => con 1em = 30px
+, rem: đơn vị đo phân trăm front-size của tử gốc (HTML) mặc định là 16px
+, vh: Đơn vị đo phân trăm chiều cao của màn hình (viewport)
+, vw: Đơn vị đo chiều rộng của màn hình
+, pt: Đơn vị đo đọ dài dựa trên điểm in ấn
+, cm: Đơn vị đo độ dài dựa trên cm

