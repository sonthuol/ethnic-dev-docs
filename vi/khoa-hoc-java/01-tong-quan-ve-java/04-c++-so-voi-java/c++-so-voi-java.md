<div style="background-color: #e7e9eb; padding: 1px 10px; border-radius: 5px; margin-bottom: 20px">

### Nội dung bài viết

1. [Điểm khác nhau và giống nhau giữa C++ với Java](#diem-khac-nhau-va-giong-nhau-giua-c++-voi-java)
2. [Ví dụ chương trình C++](#vi-du-chuong-trinh-c++)
3. [Ví dụ chương trình Java](#vi-du-chuong-trinh-java)

</div>

<div class="section" id="diem-khac-nhau-va-giong-nhau-giua-c++-voi-java"><div>

## Điểm khác nhau và giống nhau giữa C++ với Java

Có nhiều điểm khác biệt và tương đồng giữa ngôn ngữ lập trình C++ và Java. Dưới đây là danh sách những điểm khác biệt hàng đầu giữa C++ và Java.

| Điểm so sánh                            | C++                                                                                                                                                   | Java                                                                                                                                                                                                                                                      |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Nền tảng độc lập                        | C++ phụ thuộc vào nền tảng                                                                                                                            | Java độc lập với nền tảng                                                                                                                                                                                                                                 |
| Chủ yếu được sử dụng cho                | C++ chủ yếu được sử dụng để lập trình hệ thống                                                                                                        | Java chủ yếu được sử dụng để lập trình ứng dụng. Nó được sử dụng rỗng rãi trong các ứng dụng dựa trên Windows, dựa trên web, doanh nghiệp và di dộng.                                                                                                     |
| Mục tiêu thiết kế                       | C++ được thiết kế để lập trình hệ thống và ứng dụng. Đó là một phần mở rộng của ngôn ngữ lập trình C.                                                 | được thiết kế và tạo ra như một trình thông dịch cho các hệ thống in nhưng sau đó được mở rộng như một máy tính mạng hỗ trợ. Nó được thiết kế để dễ sử dụng và dễ tiếp cận với nhiều đối tượng hơn.                                                       |
| Goto                                    | C++ hỗ trợ câu lệnh goto.                                                                                                                             | Java không hỗ trợ câu lệnh goto.                                                                                                                                                                                                                          |
| Đa kế thừa                              | C++ hỗ trợ đa kế thừa                                                                                                                                 | Java không hỗ trợ đa kế thừa thông qua lớp. Nó có thể đạt được bằng cách sử dụng các giao diện trong java.                                                                                                                                                |
| Trình biên dịch và thông dịch           | C++ chỉ sử dụng trình biên dịch. C++ được biên dịch và chạy bằng trình biên dịch chuyển đổi mã nguồn thành mã máy, vì vậy C++ phụ thuộc vào nền tảng. | Java sử dụng cả trình biên dịch và trình thông dịch. Mã nguồn Java được chuyển đổi thành mã byte tại thời điểm biên dịch. Trình thông dịch thực thi mã byte này khi chạy và tạo đầu ra. Java được giải thích đó là lý do tại sao nó độc lập với nền tảng. |
| Gọi theo giá trị và gọi theo tham chiếu | C++ hỗ trợ cả gọi theo giá trị và gọi theo tham chiếu.                                                                                                | Java chỉ hỗ trợ cuộc gọi theo giá trị. Không có cuộc gọi bằng tham chiếu trong java.                                                                                                                                                                      |
| Cấu trúc và Liên minh                   | C++ hỗ trợ các cấu trúc và công đoàn.                                                                                                                 | ava chỉ hỗ trợ cuộc gọi theo giá trị. Không có cuộc gọi bằng tham chiếu trong java.                                                                                                                                                                       |
| Thread Support                          | C++ không có hỗ trợ tích hợp cho các luồng. Nó dựa vào thư viện của bên thứ ba để hỗ trợ luồng.                                                       | Java có hỗ trợ luồng tích hợp.                                                                                                                                                                                                                            |
| Documentation comment                   | C++ không hỗ trợ nhận xét tài liệu.                                                                                                                   | Java hỗ trợ tài liệu comment (/\*_ ... _/) để tạo tài liệu cho mã nguồn java.                                                                                                                                                                             |
| Virtual Keyword                         | C++ hỗ trợ từ khóa ảo để chúng ta có thể quyết định có ghi đè hàm hay không                                                                           | Java không có từ khóa ảo. Theo mặc định, chúng ta có thể ghi đè tất cả các phương thức không tĩnh. Nói cách khác, các phương thức không tĩnh theo mặc định là ảo.                                                                                         |
| dịch chuyển phải không dấu >>>          | C++ không hỗ trợ toán tử >>>.                                                                                                                         | Java hỗ trợ toán tử shift phải không dấu >>> điền số 0 ở trên cùng cho các số âm. Đối với số dương, nó hoạt động tương tự như toán tử >>.                                                                                                                 |
| Cây kế thừa                             | C++ luôn tạo cây kế thừa mới.                                                                                                                         | Java luôn sử dụng một cây kế thừa duy nhất vì tất cả các lớp đều là con của lớp Object trong Java. Lớp Object là gốc của cây kế thừa trong java.                                                                                                          |
| Phần cứng                               | C++ gần với phần cứng hơn.                                                                                                                            | Java không tương tác nhiều với phần cứng                                                                                                                                                                                                                  |
| Hướng đối tượng                         | C++ là một ngôn ngữ hướng đối tượng. Tuy nhiên, trong ngôn ngữ C, không thể có một hệ thống phân cấp gốc duy nhất.                                    | Java cũng là một ngôn ngữ hướng đối tượng. Tuy nhiên, mọi thứ (trừ các kiểu cơ bản) đều là đối tượng trong Java. Nó là một hệ thống phân cấp gốc duy nhất vì mọi thứ đều bắt nguồn từ java.lang.Object.                                                   |

Ghi chú:

- Ghi chú Java không hỗ trợ các đối số mặc định như C++.
- Java không hỗ trợ các tệp tiêu đề như C++. Java sử dụng từ khóa import để bao gồm các lớp và phương thức khác nhau.

<div class="section" id="vi-du-chuong-trinh-c++"><div>

## Ví dụ chương trình C++

File: main.cpp

```cpp
#include <iostream>
using namespace std;
int main() {
   cout << "Hello C++ Programming";
   return 0;
}
```

Kết quả:

```
Hello C++ Programming
```

<div class="section" id="vi-du-chuong-trinh-java"><div>

## Ví dụ chương trình Java

File: Simple.java

```java
class Simple{
    public static void main(String args[]){
     System.out.println("Hello Java");
    }
}
```

Kết quả:

```
Hello Java
```
