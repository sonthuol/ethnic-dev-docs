<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Đặc điểm của Java](#dac-diem-cua-java)
2. [Simple](#Simple)
3. [Object-Oriented](#Object-Oriented)
4. [Portable](#Portable)
5. [Platform independent](#Platform-independent)
6. [Secured](#Secured)
7. [Robust](#Robust)
8. [Architecture neutral](#Architecture-neutral)
9. [Interpreted](#Interpreted)
10. [High Performance](#High-Performance)
11. [Multithreaded](#Multithreaded)
12. [Distributed](#Distributed)
13. [Dynamic](#Dynamic)

</div>

<div class="section" id="dac-diem-cua-java"><div>

## Đặc điểm của Java

Mục tiêu chinh của việc tạo ra ngôn ngữ lập trình JAva là làm cho nó trở thành ngôn ngữ lập trình di dộng, đơn giản và an toàn. Ngoài ra, còn một số tính năng tuyệt vời đóng vai trò quan trọng trong sự phổ biến của ngôn ngữ này. Các tính năng của Java còn được gọi là từ thông dụng Java.

Dưới đây là danh sách các tính năng quan trọng của Java

![Features of java](https://static.javatpoint.com/images/core/java-features.png)

1. [Simple](#Simple)
2. [Object-Oriented](#Object-Oriented)
3. [Portable](#Portable)
4. [Platform independent](#Platform-independent)
5. [Secured](#Secured)
6. [Robust](#Robust)
7. [Architecture neutral](#Architecture-neutral)
8. [Interpreted](#Interpreted)
9. [High Performance](#High-Performance)
10. [Multithreaded](#Multithreaded)
11. [Distributed](#Distributed)
12. [Dynamic](#Dynamic)

<div class="section" id="Simple"><div>

## Simple (Đơn giản)

Java rất dễ học và cú pháp của nó đơn giản, rõ ràng và dễ hiểu. Theo Sun Microsystems, ngôn ngữ lập trình đơn giản vì:

- Cú pháp java thì dựa trên C++ (Để các lập trình viên học nó sang C++ dễ dàng hơn)
- Java đã loại bỏ đi nhiều tính năng phức tạp và ít được sử dụng, ví dụ như con trỏ tường minh, nạp chồng toán tử,...
- Không cần phải xoá các đối tượng không được ước tính, vì đã có Automatic Garbage Collection trong Java.

<div class="section" id="Object-Oriented"><div>

## Object-oriented (Hướng đối tượng)

Java là một ngôn ngữ lập trình hướng đối tượng. Mọi thứ trong Java đều là một đối tượng. Hướng đối tượng có nghĩa là chúng tôi tổ chức phần mềm của mình dưới dạng kết hợp nhiều loại đối tượng khác nhau thành kết hợp cả dữ liệu và hành vi.

Lập trình hướng đối tượng OOP là một phương pháp đơn giản hoá việc phát triển và bảo trì phần mềm bằng cách cung cấp một vài quy tắt.

Các khái niệm cơ bản của OOP là:

1\) Object
2\) Class
3\) Inheritance
4\) Polymorphism
5\) Abstraction
6\) Encapsulation

<div class="section" id="Platform-independent"><div>

## Plaform Independent (Nền tảng độc lập)

![Plaform Independent](https://static.javatpoint.com/images/core/platform-independent-java.png)

Java độc lập với nền tảng vì nó khác với các ngôn ngữ khác như C++, C,... Được biên dịch thành các máy cụ thể trên nền tảng trong khi Java viết một lần, chạy mọi nơi. Nền tảng là môi trường phần cứng hoặc phần mềm trong đó là chương trình chạy.

Có hai loại nền tảng dựa trên phần mềm và dựa trên phần cứng. Java cung cấp một nền tảng dựa trên phần mềm.

Nền tảng Java khác với hầu hết các nền tảng khác ở chỗ nó là nền tảng chạy trên phần mềm chạy trên các nền tảng dựa trên phần cứng khác. Nó có hai thành phần:

1\) Môi trường thực thi (Runtime Environment)
2\) API(Application Programming Interface)

Mã Java có thể được thực thi trên nhiều nền tảng, ví dụ: Windows, Linux, Sun Solaris, Mac,... Mã Java thì được trình biên dịch biên dịch và chuyển đổi thành mã byte. Mã byte này là mã độc lập với nền tảng vì nó có thể chạy trên nhiều nền thảng, tức là viết một lần, chạy mọi nơi. (Write Once and Run Anywhere - WORA)

<div class="section" id="Secured"><div>
<div class="section" id="Interpreted"><div>

## Secured (Bảo mật)

Java được biết đến nhiều nhất vì tính bảo mật của nó, với Java, chúng tôi có thể phát triển các hệ thống không có Virut. Java được bảo mật vì:

- No explicit pointer (Không có con trỏ rõ ràng)
- Java Programs run inside a virtual machine sandbox (Các chương trình Java chạy bên trong hộp cát máy ảo)

![java-security](https://static.javatpoint.com/images/core/java-security.png)

- Classloader: Classloader trong Java là một phần Java Runtime Environment (JRE) được sử dụng để tải các lớp Java vào Java Virtual Machine một cách linh hoạt. Nó tăng thêm tính bảo mật bằng cách tách gói dành cho các lớp của hệ thống tệp cục bộ khỏi các gọi được nhập từ nguồn mạng.

- ByteCode Verifier: Trình xác mình mã byte: Nó kiểm tra các đoạn mã để tìm mã bất hợp pháp có thể vi phạm quyền truy cập vào các đối tượng.

- Security Manager: It xác định những tài nguyên mà một lớp có thể truy cập, chẳng hạn như đọc và ghi vào đĩa cục bộ.

Ngôn ngữ ava cung cấp các chứng khoán này theo mặc định. Một số bảo mật cũng có thể được nhà phát triển ứng dụng cung cấp rõ ràng thông qua SSL, JAAS, Mật mã, v.v.

<div class="section" id="Robust"><div>

## Robust (Mạnh mẽ)

Khả năng khai thác Robust bằng tiếng Anh rất mạnh. Java mạnh mẽ vì:

- Nó sử dụng quản lý bộ nhớ mạnh mẽ.
- Thiếu con trỏ để tránh các vấn đề bảo mật.
- Java cung cấp tính năng thu thập rác tự động chạy trên Máy ảo Java để loại bỏ các đối tượng không còn được ứng dụng Java sử dụng nữa.
- Có cách xử lý ngoại lệ và cơ chế kiểm tra kiểu trong Java. Tất cả những điểm này làm cho Java trở nên mạnh mẽ.

<div class="section" id="Architecture-neutral"><div>

## Architecture-neutral (Kiến trúc trung lập)

Java là kiến trúc trung lập vì nó không có tính năng phụ thuộc vào việc triển khai, ví dụ: Kích thước của các kiểu nguyên thuỷ là cô định.

Trong lập trình C, kiểu dữ liệu int chiếm 2 byte bộ nhớ cho kiến ​​trúc 32 bit và 4 byte bộ nhớ cho kiến ​​trúc 64 bit. Tuy nhiên, nó chiếm 4 byte bộ nhớ cho cả kiến ​​trúc 32 và 64 bit trong Java.

<div class="section" id="Portable"><div>

## Portable

Java có tính di động vì nó tạo điều kiện cho bạn mang mã byte Java đến bất kỳ nền tảng nào. Nó không yêu cầu thực hiện bất kỳ

<div class="section" id="High-Performance"><div>

## High-performance

Java nhanh hơn các ngôn ngữ lập trình thông dịch truyền thống khác vì mã byte Java "gần" với mã gốc. Nó vẫn chậm hơn một chút so với ngôn ngữ được biên dịch (ví dụ: C++). Java là một ngôn ngữ được thông dịch, đó là lý do tại sao nó chậm hơn các ngôn ngữ được biên dịch, ví dụ: C, C++, v.v.

<div class="section" id="Distributed"><div>

## Distributed

Java được phân phối vì nó tạo điều kiện cho người dùng tạo các ứng dụng phân tán trong Java. RMI và EJB được sử dụng để tạo các ứng dụng phân tán. Tính năng này của Java giúp chúng ta có thể truy cập các tệp bằng cách gọi các phương thức từ bất kỳ máy nào trên internet.

<div class="section" id="Multithreaded"><div>

## Multi-threaded

Một thread giống như một chương trình riêng biệt, thực hiện đồng thời. Chúng ta có thể viết các chương trình Java xử lý nhiều tác vụ cùng một lúc bằng cách xác định nhiều luồng. Ưu điểm chính của đa luồng là nó không chiếm bộ nhớ cho mỗi luồng. Nó chia sẻ một vùng bộ nhớ chung. Chủ đề rất quan trọng đối với đa phương tiện, ứng dụng Web, v.v.

<div class="section" id="Dynamic"><div>

## Dynamic

Java là một ngôn ngữ động. Nó hỗ trợ tải động các lớp. Nó có nghĩa là các lớp học được tải theo yêu cầu. Nó cũng hỗ trợ các chức năng từ ngôn ngữ mẹ đẻ của nó, tức là C và C++.

Java hỗ trợ biên dịch động và quản lý bộ nhớ tự động (thu gom rác).
