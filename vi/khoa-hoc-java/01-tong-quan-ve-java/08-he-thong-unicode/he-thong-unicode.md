<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Hệ thống Unicode](#he-thong-unicode)
2. [Tại sao java sử dụng hệ thống Unicode?](#tai-sao-java-su-dung-he-thong-unicode)
3. [Vấn đề](#van-de)
4. [Giải pháp](#giai-phap)

</div>

<div class="section" id="he-thong-unicode"><div>

## Hệ thống Unicode

Unicode là bảng mã ký tự tiêu chuẩn quốc tế phổ quát có khả năng đại diện cho hầu hết các ngôn ngữ viết trên thế giới.

<div class="section" id="tai-sao-java-su-dung-he-thong-unicode"><div>

## Tại sao java sử dụng hệ thống Unicode?

Trước Unicode, có nhiều tiêu chuẩn ngôn ngữ:

- ASCII (Mã tiêu chuẩn Mỹ về trao đổi thông tin) của Hoa Kỳ.
- ISO 8859-1 cho ngôn ngữ Tây Âu.
- KOI-8 cho tiếng Nga.
- GB18030 và BIG-5 cho tiếng Trung, v.v.

<div class="section" id="van-de"><div>

## Vấn đề

Điều này gây ra hai vấn đề:

1. Một giá trị mã cụ thể tương ứng với các chữ cái khác nhau trong các tiêu chuẩn ngôn ngữ khác nhau.
2. Mã hóa cho các ngôn ngữ có bộ ký tự lớn có độ dài thay đổi. Một số ký tự phổ biến được mã hóa dưới dạng byte đơn, số khác yêu cầu hai byte trở lên.

<div class="section" id="giai-phap"><div>

## Giải pháp

Để giải quyết những vấn đề này, một tiêu chuẩn ngôn ngữ mới đã được phát triển tức là Hệ thống Unicode.
Trong unicode, ký tự chứa 2 byte nên java cũng sử dụng 2 byte cho ký tự.  
<b>giá trị thấp nhất</b>: \u0000  
<b>giá trị cao nhất</b>: \uFFFF
