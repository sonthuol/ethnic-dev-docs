<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Biến trong Java](#bien-trong-java)
2. [Biến](#bien)
3. [Các loại biến](#cac-loai-bien)
4. [Ví dụ để hiểu về loại biến trong Java](#vi-du-ve-cac-loai-bien)
5. [Ví dụ về biến Java: Tổng 2 số](#tong-hai-so)
6. [Ví dụ về biến Java: Nới rộng (Widening)](#widening)
7. [Ví dụ về biến Java: Ép kiểu [Narrowing (Typecasting)]](#ep-kieu)
8. [Ví dụ về biến Java: Interger Overflow (tràn số nguyên)](#tran-so-nguyen)
9. [Ví dụ về biến Java: Cộng 2 số với kiểu thấp](#cong-hai-so-kieu-thap)

</div>

<div class="section" id="bien-trong-java"><div>

## Biến trong Java

Một biến là một vùng chứa giá trị trong khi chương trình Java thực thi. Một biến được gán với một kiểu dữ liệu.

Biến là tên của vị trí bộ nhớ. Có ba kiểu biến trong Java: `local`, `instance` và `static`

Có 2 loại kiểu dữ liệu trong Java: Primitive (Nguyên thuỷ) and non-primitive (Không nguyên thuỷ).

<div class="section" id="bien"><div>

## Biến

Biến là tên của vùng dành riêng được phân bổ trong bộ nhớ. Nói cách khác, đó là tên của vị trí bộ nhớ. Nó là sự kết hợp "vary + able" (Khác nhau + có thể) vì vậy nó có nghĩa là giá trị của nó có thể thay đổi.

![Varibale](https://static.javatpoint.com/core/images/variable.png)

```java
int data = 100; // Ở đây data là một biến
```

<div class="section" id="cac-loai-bien"><div>

## Các loại biến

Có ba loại biến trong Java:  
1\) Biến Local (Biến cục bộ)  
2\) Biến Instance  
3\) Biến Static (Biến tĩnh)

![Types of variable](https://www.boardinfinity.com/blog/content/images/2022/12/Your-paragraph-text--69--1.jpg)

1\) Biến Local (Biến cục bộ)

Một biến được khai báo trong phần thân của phương thức được gọi là biến cục bộ. Bạn chỉ có thể sử dụng biến này trong phương thức đó và các phương thức khác trong lớp thậm chí không biết rằng biến đó tồn tại.

Biến cục bộ không thể được xác định bằng từ khoá `static`

2\) Biến Instance

Một biến được khai báo bên trong lớp nhưng bên ngoài phần thân của phương thức, được gọi là biến instance. Nó không được khai báo là `static`.

Nó được gọi là biến instance vì giá trị của nó dành riêng cho từng instance và không được chia sẻ giữa các thể hiện

3\) Biến Static (Biến tĩnh)

Một biến được khai báo là static được gọi là biến static. Nó không phải là biến local. Bạn có thể tạo một bản sao duy nhất của biến static và chia sẻ nó giữa tất các instance của lớp.

Việc cấp phát bộ nhớ cho các biến tĩnh chỉ xảy ra một lần khi lớp được tải vào bộ nhớ.

<div class="section" id="vi-du-ve-cac-loai-bien"><div>

## Ví dụ để hiểu về loại biến trong Java

```java
public class Example {

    static String staticVariable = "This is static variable";

    public void method() {
        String localVariable = "This is local variable";
    }

    public static void main(String args[]) {
        String instanceVariable = "This is instance varibale";
    }

}

```

<div class="section" id="tong-hai-so"><div>

## Ví dụ về biến Java: Tổng 2 số

```java
public class Example {

    public static void main(String args[]) {
        int a = 10;
        int b = 10;
        int sum = a + b;
        System.out.println(sum);
    }

}
```

Kết quả:

```
20
```

<div class="section" id="widening"><div>

## Ví dụ về biến Java: Nới rộng (Widening)

Widening: Là quá trình làm tròn số từ kiểu dữ liệu có kích thước nhỏ hơn sang kiểu dữ liệu có kích thước lớn hơn.

```java
public class Example {

    public static void main(String args[]) {
        int a = 10;
        float f = a;
        System.out.println(a);
        System.out.println(f);
    }

}
```

Kết quả:

```
10
10.0
```

<div class="section" id="ep-kieu"><div>

## Ví dụ về biến Java: Ép kiểu [Narrowing (Typecasting)]

Là đúc bao gồm việc chuyển đổi một loại lớn hơn sang một loại nhỏ hơn. Đây là trình tự thu hẹp ép kiểu: double -> float -> long -> int -> char -> short -> byte.

```java
public class Example {

    public static void main(String args[]) {
        float f=10.5f;
        //int a=f;//Compile time error
        int a=(int)f;
        System.out.println(f);
        System.out.println(a);
    }

}
```

Kết quả:

```
10.5
10
```

<div class="section" id="tran-so-nguyen"><div>

## Ví dụ về biến Java: Interger Overflow (tràn số nguyên)

Interger Overflow (tràn số nguyên) là một lỗi tràn số học, xảy ra khi kết quả của một phép toán số nguyên không nằm trong giới hạn bộ nhớ. Việc này không dẫn đến lỗi chương trình mà thường đưa ra những kết quả không mong muốn.

```java
public class Example {

    public static void main(String args[]) {
        //Overflow
        int a=130;
        byte b=(byte)a;
        System.out.println(a);
        System.out.println(b);
    }

}
```

Kết quả:

```
130
-126
```

<div class="section" id="cong-hai-so-kieu-thap"><div>

## Ví dụ về biến Java: Cộng 2 số với kiểu thấp

```java
public class Example {

    public static void main(String args[]) {
        byte a=10;
        byte b=10;
        //byte c=a+b;//Compile Time Error: because a+b=20 will be int
        byte c=(byte)(a+b);
        System.out.println(c);
    }

}
```

Kết quả:

```
20
```
