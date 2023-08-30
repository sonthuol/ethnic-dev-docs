<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Chương trình Java đầu tiên | ví dụ về Hello World](#hello-world)
2. [Yêu cầu đối với ví dụ về Java Hello World](#yeu-cau-doi-voi-vi-du-ve-java-hello-world)
3. [Tạo ví dụ Hello World](#tao-vi-du-hello-world)
4. [Luồng biên dịch](#luong-bien-dich)
5. [Các tham số được sử dụng trong Chương trình Java đầu tiên](#cac-tham-so-duoc-duoc-su-dung-trong-chuong-trinh-java-dau-tien)

</div>

<div class="section" id="hello-world"><div>

## Chương trình Java đầu tiên | ví dụ về Hello World

Trong phần này, chúng ta học viết như thế nào một chương trình Java đầu tiên. Chúng ta có viết một chương trình Hello World đơn giản một cách dễ dàng sau khi chúng ta tải JDK.

Để tạo một chương chương trình Hello World đơn giản, bạn cần phải tạo một class chứa một phương thức main.
Đầu tiên, chúng ta hãy tìm hiểu hiểu yêu cầu.

<div class="section" id="yeu-cau-doi-voi-vi-du-ve-java-hello-world"><div>

## Yêu cầu đối với ví dụ về Java Hello World

Đề thực thi mọi chương trình Java, phần mềm hoặc ứng dụng sau phải được cài đặt đúng cách.

- Tải JDK, nếu bạn chưa tải nó, hãy truy cập [Tải JDK](http://www.oracle.com/technetwork/java/javase/downloads/index.html) và hãy tải nó.
- Đặt đường dẫn của thư mục jdk/bin
- Tạo chương trình Java
- Biên dịch và chạy chương trình Java

<div class="section" id="tao-vi-du-hello-world"><div>

## Tạo ví dụ Hello World

Nào hãy tạo một chương trình Hello World:

```java
class Simple {
    public static void main(String args[]) {
        System.out.println("Hello Java");
    }
}
```

Lưu đoạn mã trên vào file Simple.Java

Để biên dịch

```cmd
javac Simple.java
```

Để thực thi

```cmd
java Simple
```

Kết quả:

```
Hello Java
```

<div class="section" id="luong-bien-dich"><div>

### Luồng biên dịch

Khi chúng ta biên dịch chương trình bằng công cụ Javac, trình biên dịch Java sẽ chuyển đổi thành mã byte.

![Java Complier](https://prepbytes-misc-images.s3.ap-south-1.amazonaws.com/assets/1679044159052-1-01%20%2811%29.png)

<div class="section" id="cac-tham-so-duoc-duoc-su-dung-trong-chuong-trinh-java-dau-tien"><div>

## Các tham số được sử dụng trong Chương trình Java đầu tiên

Nào chúng ta hãy xem ý nghĩa của `class`, `public`, `static`, `void`, `main`, `String[]`, `System.out.println()`.

- `class` là một từ khoá được sử dụng để khai báo một class trong java.
- `public` là một từ khoá cho phép quyền truy cập, hay còn được gọi là access modifiter đại diện cho khả năng hiển thị. Ở đây nó có nghĩa là hiển thị cho tất cả mọi chỗ khi mình truy cập.

- `static` là một từ khóa. Nếu chúng ta khai báo bất kỳ phương thức nào là tĩnh thì nó được gọi là phương thức tĩnh. Ưu điểm cốt lõi của phương thức tĩnh là không cần tạo đối tượng để gọi phương thức tĩnh. Phương thức main() được thực thi bởi JVM, do đó nó không yêu cầu tạo một đối tượng để gọi phương thức main(). Vì vậy, nó tiết kiệm bộ nhớ.

- `void` là kiểu trả về của phương thức (method). Nó có nghĩa là không trả về bất kỳ giá trị nào.

- `main` đại diện cho điểm bắt đầu của chương trình.

- `String[]` args hoặc `String args[]` được sử dụng cho đối số dòng lệnh. Chúng ta sẽ thảo luận về nó trong phần tới.

- `System.out.println()` được sử dụng để in câu lệnh. Ở đây System là một lớp, out là một đối tượng của lớp PrintStream, println() là một phương thức của lớp PrintStream. Chúng ta sẽ thảo luận về hoạt động nội bộ của câu lệnh `System.out.println()` trong phần sắp tới.
