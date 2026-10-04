# Bài tập Python cơ bản

# Hướng dẫn làm bài

Các bài tập được sắp xếp từ cơ bản đến nâng cao, tương ứng với các nội dung đã học:

1. Làm quen với Python
2. Biến và kiểu dữ liệu
3. Cấu trúc điều kiện
4. Vòng lặp
5. Hàm

Người học nên tự viết chương trình, chạy thử và kiểm tra kết quả trước khi xem gợi ý.

---

# Phần 1. Làm quen với Python

## Bài 1. Xin chào Python

Viết chương trình hiển thị:

```text
Hello, Python!
```

---

## Bài 2. Giới thiệu bản thân

Sử dụng `print()` để hiển thị:

```text
Xin chào!
Tôi đang học Python.
Tôi muốn trở thành lập trình viên.
```

---

## Bài 3. In nhiều thông tin

Viết chương trình hiển thị:

```text
Python
Programming
STEM
Robotics
```

Mỗi nội dung nằm trên một dòng.

---

# Phần 2. Biến và kiểu dữ liệu

## Bài 4. Thông tin học sinh

Tạo các biến:

```python
name
age
score
is_student
```

Gán giá trị phù hợp và hiển thị ra màn hình.

Ví dụ:

```text
Tên: An
Tuổi: 12
Điểm: 8.5
Là học sinh: True
```

---

## Bài 5. Phép tính cơ bản

Cho:

```python
a = 10
b = 5
```

Tính và hiển thị:

- Tổng
- Hiệu
- Tích
- Thương

---

## Bài 6. Kiểm tra kiểu dữ liệu

Tạo các biến:

```python
number = 10
score = 8.5
name = "An"
is_student = True
```

Sử dụng `type()` để kiểm tra kiểu dữ liệu của từng biến.

---

## Bài 7. Tính diện tích hình chữ nhật

Cho:

```python
length = 10
width = 5
```

Tính diện tích hình chữ nhật.

Công thức:

```text
Diện tích = chiều dài × chiều rộng
```

Kết quả mong muốn:

```text
Diện tích: 50
```

---

# Phần 3. Cấu trúc điều kiện

## Bài 8. Kiểm tra số dương

Cho:

```python
number = 10
```

Kiểm tra xem số đó là:

- Số dương
- Số âm
- Bằng 0

---

## Bài 9. Kiểm tra độ tuổi

Cho:

```python
age = 16
```

Nếu tuổi từ 18 trở lên, hiển thị:

```text
Đủ tuổi
```

Ngược lại:

```text
Chưa đủ tuổi
```

---

## Bài 10. Xếp loại điểm

Cho:

```python
score = 8
```

Xếp loại:

| Điểm | Kết quả |
|---|---|
| `>= 9` | Xuất sắc |
| `>= 7` | Tốt |
| `>= 5` | Đạt |
| `< 5` | Chưa đạt |

---

## Bài 11. Kiểm tra số chẵn

Cho:

```python
number = 12
```

Kiểm tra xem số đó có phải số chẵn hay không.

Gợi ý:

```python
number % 2
```

---

## Bài 12. Tìm số lớn hơn

Cho:

```python
a = 15
b = 20
```

Sử dụng `if` để xác định số nào lớn hơn.

---

# Phần 4. Vòng lặp

## Bài 13. In các số từ 1 đến 10

Sử dụng vòng lặp `for` để hiển thị:

```text
1
2
3
...
10
```

---

## Bài 14. In số chẵn

Sử dụng vòng lặp để in các số chẵn từ `2` đến `20`.

Kết quả:

```text
2
4
6
8
10
12
14
16
18
20
```

---

## Bài 15. Tính tổng

Tính tổng các số từ `1` đến `100`.

Kết quả:

```text
5050
```

---

## Bài 16. Bảng cửu chương

Viết chương trình in bảng cửu chương của số `5`.

Kết quả:

```text
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
5 x 4 = 20
5 x 5 = 25
5 x 6 = 30
5 x 7 = 35
5 x 8 = 40
5 x 9 = 45
5 x 10 = 50
```

---

## Bài 17. Đếm số chẵn

Cho:

```python
numbers = [1, 4, 7, 8, 10, 13, 16]
```

Sử dụng vòng lặp để đếm số lượng số chẵn.

---

## Bài 18. Tìm số lớn nhất

Cho:

```python
numbers = [5, 12, 3, 20, 8]
```

Sử dụng vòng lặp để tìm số lớn nhất.

---

## Bài 19. Vòng lặp `while`

Sử dụng `while` để in các số từ `1` đến `10`.

---

# Phần 5. Hàm

## Bài 20. Hàm chào hỏi

Tạo hàm:

```python
say_hello()
```

Hàm hiển thị:

```text
Hello Python!
```

---

## Bài 21. Hàm chào theo tên

Tạo hàm:

```python
greet(name)
```

Ví dụ:

```python
greet("An")
```

Kết quả:

```text
Xin chào An
```

---

## Bài 22. Hàm tính tổng

Tạo hàm:

```python
add(a, b)
```

Hàm trả về tổng của hai số.

Ví dụ:

```python
result = add(10, 20)
print(result)
```

Kết quả:

```text
30
```

---

## Bài 23. Hàm tính bình phương

Tạo hàm:

```python
square(number)
```

Hàm trả về bình phương của một số.

Ví dụ:

```python
print(square(5))
```

Kết quả:

```text
25
```

---

## Bài 24. Hàm kiểm tra số chẵn

Tạo hàm:

```python
is_even(number)
```

Hàm trả về `True` nếu số là số chẵn và `False` nếu là số lẻ.

---

## Bài 25. Hàm kiểm tra kết quả

Tạo hàm:

```python
check_result(score)
```

Quy ước:

- Điểm từ 5 trở lên → `"Đạt"`
- Điểm dưới 5 → `"Chưa đạt"`

---

# Phần 6. Bài tập tổng hợp

## Bài 26. Máy tính đơn giản

Viết chương trình cho phép thực hiện:

- Cộng
- Trừ
- Nhân
- Chia

với hai số.

Gợi ý cấu trúc:

```python
def add(a, b):
    ...

def subtract(a, b):
    ...

def multiply(a, b):
    ...

def divide(a, b):
    ...
```

---

## Bài 27. Quản lý điểm học sinh

Viết chương trình:

1. Lưu tên học sinh.
2. Lưu điểm Toán, Văn và Anh.
3. Tính điểm trung bình.
4. Xếp loại kết quả.
5. Hiển thị thông tin học sinh.

Có thể chia chương trình thành các hàm:

```python
calculate_average()
check_result()
show_student()
```

---

## Bài 28. Trò chơi đoán số

Viết chương trình cho người chơi đoán một số.

Ví dụ:

```text
Hãy đoán số từ 1 đến 10: 5
Số cần tìm lớn hơn.

Hãy đoán số từ 1 đến 10: 8
Chính xác!
```

Gợi ý sử dụng:

```text
while
if
```

---

# Phần 7. Thử thách

## Bài 29. Kiểm tra số nguyên tố

Viết chương trình kiểm tra một số có phải số nguyên tố hay không.

Ví dụ:

```text
Nhập số: 17
17 là số nguyên tố.
```

Gợi ý: sử dụng vòng lặp để kiểm tra các số có thể chia hết cho số cần kiểm tra.

---

## Bài 30. Menu chương trình

Xây dựng chương trình có menu:

```text
===== MENU =====
1. Tính tổng
2. Kiểm tra số chẵn/lẻ
3. Tính bình phương
4. Thoát
```

Người dùng chọn chức năng và chương trình thực hiện chức năng tương ứng.

Gợi ý sử dụng:

```text
while
if / elif / else
function
```

---

# Phần 8. Dự án nhỏ

## Quản lý thông tin học sinh

Xây dựng một chương trình đơn giản để quản lý thông tin học sinh.

Chương trình cần có:

### Thông tin

- Họ tên
- Tuổi
- Điểm Toán
- Điểm Văn
- Điểm Anh

### Chức năng

1. Nhập thông tin.
2. Tính điểm trung bình.
3. Xếp loại học tập.
4. Hiển thị thông tin.
5. Thoát chương trình.

Có thể tổ chức chương trình bằng các hàm:

```python
def input_student():
    ...

def calculate_average():
    ...

def check_result():
    ...

def show_student():
    ...
```

---

# Checklist hoàn thành

| Nội dung | Hoàn thành |
|---|---|
| In dữ liệu bằng `print()` | ☐ |
| Tạo và sử dụng biến | ☐ |
| Sử dụng `int`, `float`, `str`, `bool` | ☐ |
| Sử dụng `if` | ☐ |
| Sử dụng `if...else` | ☐ |
| Sử dụng `if...elif...else` | ☐ |
| Sử dụng `for` | ☐ |
| Sử dụng `while` | ☐ |
| Sử dụng `break` | ☐ |
| Sử dụng `continue` | ☐ |
| Tạo hàm bằng `def` | ☐ |
| Truyền tham số vào hàm | ☐ |
| Sử dụng `return` | ☐ |
| Kết hợp nhiều kiến thức | ☐ |

> **Mục tiêu:** Không chỉ hoàn thành bài tập, hãy cố gắng tự giải quyết vấn đề, thử nhiều trường hợp đầu vào và kiểm tra kết quả của chương trình.
