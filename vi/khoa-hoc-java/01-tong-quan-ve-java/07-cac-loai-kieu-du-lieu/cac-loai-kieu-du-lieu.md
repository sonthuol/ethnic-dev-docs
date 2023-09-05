<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Các kiểu dữ liệu trong Java](#cac-kieu-du-lieu-trong-java)
2. [Các kiểu dữ liệu nguyên thuỷ của Java](#cac-kieu-du-lieu-nguyen-thuy-cua-java)
3. [Kiểu dữ liệu boolean](#kieu-du-lieu-boolean)
4. [Kiểu dữ liệu byte](#kieu-du-lieu-byte)
5. [Kiểu dữ liệu short](#kieu-du-lieu-short)
6. [Kiểu dữ liệu int](#kieu-du-lieu-int)
7. [Kiểu dữ liệu long](#kieu-du-lieu-long)
8. [Kiểu dữ liệu float](#kieu-du-lieu-float)
9. [Kiểu dữ liệu double](#kieu-du-lieu-double)
10. [Kiểu dữ liệu char](#kieu-du-lieu-char)
11. [Tại sao char sử dụng 2 byte trong java và \u0000 là gì?](#tai-sao-char-su-dung-2-byte-trong-java)

</div>

<div class="section" id="cac-kieu-du-lieu-trong-java"><div>

## Các kiểu dữ liệu trong Java

Các kiểu dữ liệu chỉ định các kích thước và giá trị khác nhau có thể lưu trữ trong biến. Có 2 kiểu dữ liệu trong trong Java:

1\) Các kiểu dữ liệu nguyên thuỷ (Primitive data types): Các kiểu dữ liệu nguyên thuỷ gồm có boolean, char, byte, short, int, long, float and double.

2\) Các kiểu dữ liệu không nguyên thuỷ (Non-primitive): Các kiểu dữ liệu không nguyên thuỷ gồm có Class, Interfaces, and Arrays

<div class="section" id="cac-kieu-du-lieu-nguyen-thuy-cua-java"><div>

## Các kiểu dữ liệu nguyên thuỷ của Java

Trong ngôn ngữ Java, các kiểu dữ liệu nguyên thuỷ là các khối xây dựng của các thao tác dữ liệu. Đây là kiểu dữ liệu cơ bản nhất có sẵn trong ngôn ngữ Java.

`Ghi chú: Java là một ngôn ngữ lập trình kiểu tĩnh. Điều đó có nghĩa là tất cả các biến phải được khai báo trước khi sử dụng. Đó là lý do tại sao chúng ta cần phải khai báo kiểu và tên biến.`

Có 8 loại kiểu dữ liệu nguyên thuỷ:

1\) boolean data type  
 2\) byte data type  
 3\) char data type  
 4\) short data type  
 5\) int data type  
 6\) long data type  
 7\) float data type  
 8\) double data type

![primitive data type](https://www.janbasktraining.com/community/uploads/de0c73eef3741d11ea8de8fbed23dc87.png)

| Kiểu dữ liệu | Giá trị mặc định | Kích thước mặc định |
| ------------ | ---------------- | ------------------- |
| boolean      | false            | 1 bit               |
| char         | '\u0000'         | 2 byte              |
| byte         | 0                | 1 byte              |
| short        | 0                | 2 byte              |
| int          | 0                | 4 byte              |
| long         | 0L               | 8 byte              |
| float        | 0.0f             | 4 byte              |
| double       | 0.0d             | 8 byte              |

<div class="section" id="kieu-du-lieu-boolean"><div>

## Kiểu dữ liệu Boolean

Kiểu dữ này dùng để lưu 2 giá trị: `true` hoặc `false`. Kiểu dữ liệu này được sử dụng cho các cờ cơ bản hoặc các điều kiện true/false.

Kiểu dữ liệu `boolean` chỉ định một bit thông tin. Nhưng không thể xác định chính xác "kích thước" của nó

Ví dụ:

```java
boolean isTrue = true;
boolean isFalse = false;
```

<div class="section" id="kieu-du-lieu-byte"><div>

## Kiểu dữ liệu byte

Kiểu dữ liệu này là một ví dụ về kiểu dữ liệu nguyên thuỷ. Đó là số nguyên bù 2 có dấu 8 bit. Phạm vi giá trị của nó nằm trong khoảng -128 đến 127. Giá trị nhỏ nhất là -128, giá trị lớn nhất là 127 và giá trị mặc định là 0

Kiểu dữ liệu byte được sử dụng để lưu bộ nhớ trong các mảng lớn, nơi cần tiết kiệm bộ nhớ nhất.  
Ví dụ:

```java
byte a = 10;
byte b = -10;
```

<div class="section" id="kieu-du-lieu-short"><div>

## Kiểu dữ liệu short

Kiểu dữ liệu short là số nguyên bù hai có dấu 16 bit. Phạm vi giá trị của nó nằm trong khoảng từ -32.768 đến 32.767 (đã bao gồm). Giá trị tối thiểu của nó là -32.768 và giá trị tối đa là 32.767. Giá trị mặc định của nó là 0.

Kiểu dữ liệu short cũng có thể được sử dụng để tiết kiệm bộ nhớ giống như kiểu dữ liệu byte. Kiểu dữ liệu short nhỏ hơn 2 lần so với số nguyên.

Ví dụ:

```java
short a = 5000;
short b = -5000;
```

<div class="section" id="kieu-du-lieu-int"><div>

## Kiểu dữ liệu int

Kiểu dữ liệu int là số nguyên bù hai có dấu 32 bit. Phạm vi giá trị của nó nằm trong khoảng - 2.147.483.648 (-2^31) đến 2.147.483.647 (2^31 -1) (đã bao gồm). Giá trị tối thiểu của nó là - 2.147.483.648 và giá trị tối đa là 2.147.483.647. Giá trị mặc định của nó là 0.

Kiểu dữ liệu int thường được sử dụng làm kiểu dữ liệu mặc định cho các giá trị tích phân trừ khi không có vấn đề gì về bộ nhớ.

Ví dụ:

```java
int a = 100000;
int b = -100000;
```

<div class="section" id="kieu-du-lieu-long"><div>

## Kiểu dữ liệu long

Kiểu dữ liệu long là số nguyên bù hai 64 bit. Phạm vi giá trị của nó nằm trong khoảng từ -9,223,372,036,854,775,808(-2^63) đến 9,223,372,036,854,775,807(2^63 -1)(đã bao gồm).

Giá trị tối thiểu của nó là - 9,223,372,036,854,775,808 và giá trị tối đa là 9,223,372,036,854,775,807. Giá trị mặc định của nó là 0. Kiểu dữ liệu long được sử dụng khi bạn cần một phạm vi giá trị nhiều hơn những giá trị do int cung cấp.

Ví dụ:

```java
long a = 100000L;
long b = -100000L;
```

<div class="section" id="kieu-du-lieu-float"><div>

## Kiểu dữ liệu float

Kiểu dữ liệu float là dấu phẩy động IEEE 754 32-bit có độ chính xác đơn. Phạm vi giá trị của nó là không giới hạn. Bạn nên sử dụng float (thay vì double) nếu bạn cần lưu bộ nhớ trong mảng lớn các số dấu phẩy động.

Kiểu dữ liệu float không bao giờ được sử dụng cho các giá trị chính xác, chẳng hạn như tiền tệ. Giá trị mặc định của nó là 0,0F.

Ví dụ:

```java
float f1 = 234.5f
```

<div class="section" id="kieu-du-lieu-double"><div>

## Kiểu dữ liệu double

Kiểu dữ liệu double là điểm nổi IEEE 754 64-bit có độ chính xác kép. Phạm vi giá trị của nó là không giới hạn. Kiểu dữ liệu double thường được sử dụng cho các giá trị thập phân giống như float. Kiểu dữ liệu double cũng không bao giờ được sử dụng cho các giá trị chính xác, chẳng hạn như tiền tệ. Giá trị mặc định của nó là 0,0d.

Ví dụ:

```java
double d1 = 12.3
```

<div class="section" id="kieu-du-lieu-char"><div>

## Kiểu dữ liệu char

Kiểu dữ liệu char là một ký tự Unicode 16 bit. Phạm vi giá trị của nó nằm trong khoảng từ '\u0000' (hoặc 0) đến '\uffff' (hoặc bao gồm 65.535). Kiểu dữ liệu char được sử dụng để lưu trữ các ký tự.

Ví dụ:

```java
char letterA = 'A'
```

<div class="section" id="tai-sao-char-su-dung-2-byte-trong-java"><div>

## Tại sao char sử dụng 2 byte trong java và \u0000 là gì?

Đó là vì java sử dụng hệ thống Unicode chứ không phải hệ thống mã ASCII. \u0000 là phạm vi thấp nhất của hệ thống Unicode. Để có được lời giải thích chi tiết về Unicode, hãy truy cập trang tiếp theo.
