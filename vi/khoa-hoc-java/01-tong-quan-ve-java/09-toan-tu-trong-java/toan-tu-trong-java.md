<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Toán tử trong Java](#toan-tu-trong-java)
2. [Toán tử một ngôi](#toan-tu-mot-ngoi)
3. [Toán tử số học](#toan-tu-so-hoc)
4. [Toán tử dịch chuyển trái](#toan-tu-dich-chuyen-trai)
5. [Toán tử dịch chuyển phải](#toan-tu-dich-chuyen-phai)
6. [Toán tử ba ngôi](#toan-tu-ba-ngoi)
7. [Toán tử gán](#toan-tu-gan)

</div>

<div class="section" id="toan-tu-trong-java"><div>

## Toán tử trong Java

Toán tử trong Java là ký hiệu dùng để thực hiện các phép toán:
Ví dụ: +, -, \*, / etc.

Có nhiều loại toán tử trong Java được đưa ra dưới đây:

- Toán tử một ngôi (Unany Operator)
- Toán tử số học (Arithmetic Operator)
- Toán tử dịch chuyển (Shift Operator)
- Toán tử quan hệ (Relational Operator)
- Toán tử Bitwise (Bitwise Operator)
- Toán tử logic (Logical Operator)
- Toán tử ba ngôi (Ternary Operator and)
- Toán tử gán (Assignment Opertor)

<div class="section" id="toan-tu-mot-ngoi"><div>

## Toán tử một ngôi

Các toán tử một ngôi trong Java chỉ yêu cầu một toán hạng. Toán tử một ngôi được sử dụng để thực hiện các phép toán khác nhau, ví dụ:

- Tăng/giảm một giá trị
- Phủ định một biểu thức
- Đảo ngược giá trị của một boolean

## Ví dụ về toán tử một ngội: ++ và --

```java
public class Example {
    public static void main (String args[]) {
        int x = 10;
        System.out.println(x++);//10 (11)
        System.out.println(++x);//12
        System.out.println(x--);//12 (11)
        System.out.println(--x);//10
    }
}
```

Kết quả:

```
10
12
12
10
```

## Ví dụ 2 về toán tử một ngội: ++ và --

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=10;
        System.out.println(a++ + ++a);//10+12=22
        System.out.println(b++ + b++);//10+11=21
    }
}
```

Kết quả:

```
22
21
```

## Ví dụ về toán tử một ngội: ~ and !

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=-10;
        boolean c=true;
        boolean d=false;
        System.out.println(~a);//-11 (minus of total positive value which starts from 0)
        System.out.println(~b);//9 (positive of total minus, positive starts from 0)
        System.out.println(!c);//false (opposite of boolean value)
        System.out.println(!d);//true
    }
}
```

Kết quả:

```
-11
9
false
true
```

<div class="section" id="toan-tu-so-hoc"><div>

## Toán tử số học

Toán tử số học được sử dụng để cộng, trừ, nhân, chia. Chúng hoạt động như các phép toán cơ bản.

## Ví dụ về toán tử số học

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=5;
        System.out.println(a+b);//15
        System.out.println(a-b);//5
        System.out.println(a*b);//50
        System.out.println(a/b);//2
        System.out.println(a%b);//0
    }
}
```

Kết quả:

```
15
5
50
2
0
```

```java
public class Example {
    public static void main (String args[]) {
        System.out.println(10*10/5+3-1*4/2);
    }
}
```

Kết quả:

```
21
```

<div class="section" id="toan-tu-dich-chuyen-trai"><div>

## Toán tử dịch chuyển trái

Toán tử dịch chuyển trái << trong Java được sử dụng để dịch chuyển tất cả các bit trong một giá trị sang bên trái sau một số lần xác định.

## Ví dụ về toán tử dịch chuyển trái

```java
public class Example {
    public static void main (String args[]) {
        System.out.println(10<<2);//10*2^2=10*4=40
        System.out.println(10<<3);//10*2^3=10*8=80
        System.out.println(20<<2);//20*2^2=20*4=80
        System.out.println(15<<4);//15*2^4=15*16=240
    }
}
```

Kết quả:

```
240
80
80
240
```

<div class="section" id="toan-tu-dich-chuyen-phai"><div>

## Toán tử dịch chuyển phải

Toán tử dịch chuyển phải >> được sử dụng để di chuyển giá trị của toán hạng bên trái sang phải theo số bit được chỉ định bởi toán hạng bên phải.

## Ví dụ về toán tử dịch chuyển phải

```java
public class Example {
    public static void main (String args[]) {
        System.out.println(10>>2);//10/2^2=10/4=2
        System.out.println(20>>2);//20/2^2=20/4=5
        System.out.println(20>>3);//20/2^3=20/8=2
    }
}
```

Kết quả:

```
2
5
2
```

## Ví dụ về toán tử dịch chuyển: >> vs >>>

```java
public class Example {
    public static void main (String args[]) {
        //For positive number, >> and >>> works same
        System.out.println(20>>2);
        System.out.println(20>>>2);
        //For negative number, >>> changes parity bit (MSB) to 0
        System.out.println(-20>>2);
        System.out.println(-20>>>2);
    }
}
```

Kết quả:

```
5
5
-5
1073741819
```

## Ví dụ về toán tử AND: Logic && và Bitwise &

Toán tử logic && không kiểm tra điều thứ 2 nếu điều kiện đầu tiên sai. Nó chỉ kiểm tra điều kiện thứ 2 nếu điều kiện đầu tiên đúng. Toán tử bitwise & luôn kiểm tra cả 2 điều kiện xem điều kiện đầu tiên là đúng hay sai.

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=5;
        int c=20;
        System.out.println(a<b&&a<c);//false && true = false
        System.out.println(a<b&a<c);//false & true = false
    }
}
```

Kết quả:

```
false
false
```

## Ví dụ về toán tử AND: Logic && với Bitwise &

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=5;
        int c=20;
        System.out.println(a<b&&a++<c);//false && true = false
        System.out.println(a);//10 because second condition is not checked
        System.out.println(a<b&a++<c);//false && true = false
        System.out.println(a);//11 because second condition is checked
    }
}
```

Kết quả:

```
false
10
false
11
```

## Ví dụ về toán tử OR: Logic || và Bitwise |

Hợp lý || toán tử không kiểm tra điều kiện thứ hai nếu điều kiện thứ nhất đúng. Nó chỉ kiểm tra điều kiện thứ hai nếu điều kiện đầu tiên sai.

Bitwise | toán tử luôn kiểm tra cả hai điều kiện xem điều kiện đầu tiên là đúng hay sai.

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=5;
        int c=20;
        System.out.println(a>b||a<c);//true || true = true
        System.out.println(a>b|a<c);//true | true = true
        //|| vs |
        System.out.println(a>b||a++<c);//true || true = true
        System.out.println(a);//10 because second condition is not checked
        System.out.println(a>b|a++<c);//true | true = true
        System.out.println(a);//11 because second condition is checked
    }
}
```

Kết quả:

```
true
true
true
10
true
11
```

<div class="section" id="toan-tu-ba-ngoi"><div>

## Toán tử ba ngôi

Toán tử ba ngôi được sử dụng thay thế một dòng cho câu lệnh if-then-else và được sử dụng rất nhiều trong lập trình Java. Đây là toán tử điều kiện duy nhất có ba toán hạng.

## Ví dụ về toán tử ba ngôi

```java
public class Example {
    public static void main (String args[]) {
        int a=2;
        int b=5;
        int min=(a<b)?a:b;
        System.out.println(min);
    }
}
```

Kết quả:

```
2
```

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=5;
        int min=(a<b)?a:b;
        System.out.println(min);
    }
}
```

Kết quả:

```
5
```

<div class="section" id="toan-tu-gan"><div>

## Toán tử gán

Toán tử gán trong Java là một trong những toán tử phổ biến nhất. Nó được sử dụng để gán giá trị ở bên phải cho toán hạng ở bên trái.

## Ví dụ về toán tử gán

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        int b=20;
        a+=4;//a=a+4 (a=10+4)
        b-=4;//b=b-4 (b=20-4)
        System.out.println(a);
        System.out.println(b);
    }
}
```

Kết quả:

```
14
16
```

## Ví dụ về toán tử gán

```java
public class Example {
    public static void main (String args[]) {
        int a=10;
        a+=3;//10+3
        System.out.println(a);
        a-=4;//13-4
        System.out.println(a);
        a*=2;//9*2
        System.out.println(a);
        a/=2;//18/2
        System.out.println(a);
    }
}
```

Kết quả:

```
13
9
18
9
```

## Ví dụ về toán tử gán: Cộng ngắn

```java
public class Example {
    public static void main (String args[]) {
        short a=10;
        short b=10;
        //a+=b;//a=a+b internally so fine
        a=a+b;//Compile time error because 10+10=20 now int
        System.out.println(a);
    }
}
```

Kết quả:

```
Compile time error
```

```java
public class Example {
    public static void main (String args[]) {
        short a=10;
        short b=10;
        a=(short)(a+b);//20 which is int now converted to short
        System.out.println(a);
    }
}
```

Kết quả:

```
20
```
