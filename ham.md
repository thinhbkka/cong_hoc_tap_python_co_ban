# Hàm trong Python

## 1. Mục tiêu bài học

Sau bài học này, người học có thể:

- Hiểu hàm là gì và tại sao cần sử dụng hàm.
- Biết cách định nghĩa một hàm bằng `def`.
- Biết cách gọi hàm.
- Biết cách truyền tham số vào hàm.
- Hiểu giá trị trả về bằng `return`.
- Biết cách sử dụng hàm với nhiều tham số.
- Vận dụng hàm để tổ chức chương trình thành các phần nhỏ, dễ quản lý.

---

## 2. Hàm là gì?

**Hàm (function)** là một nhóm câu lệnh được đặt tên và có thể được gọi để thực hiện một công việc cụ thể.

Ví dụ, thay vì viết lại nhiều lần các câu lệnh tính tổng, chúng ta có thể tạo một hàm để thực hiện công việc đó.

Hàm giúp chương trình:

- Dễ đọc hơn.
- Dễ kiểm tra và sửa lỗi.
- Có thể tái sử dụng.
- Chia một chương trình lớn thành nhiều phần nhỏ.

---

## 3. Tạo một hàm

Trong Python, sử dụng từ khóa `def` để định nghĩa hàm.

Cú pháp:

```python
def ten_ham():
    cau_lenh
```

Ví dụ:

```python
def say_hello():
    print("Hello, Python!")
```

Ở đây:

- `def` dùng để định nghĩa hàm.
- `say_hello` là tên hàm.
- `()` chứa tham số của hàm.
- Các câu lệnh bên trong hàm phải được thụt lề.

---

## 4. Gọi hàm

Sau khi định nghĩa, hàm chỉ được thực hiện khi được gọi.

```python
def say_hello():
    print("Hello, Python!")

say_hello()
```

Kết quả:

```text
Hello, Python!
```

Có thể gọi một hàm nhiều lần:

```python
def say_hello():
    print("Hello!")

say_hello()
say_hello()
say_hello()
```

Kết quả:

```text
Hello!
Hello!
Hello!
```

---

## 5. Hàm có tham số

Tham số cho phép truyền dữ liệu vào hàm.

Cú pháp:

```python
def ten_ham(tham_so):
    cau_lenh
```

Ví dụ:

```python
def greet(name):
    print("Hello", name)

greet("An")
greet("Binh")
```

Kết quả:

```text
Hello An
Hello Binh
```

Trong ví dụ trên:

- `name` là tham số.
- `"An"` và `"Binh"` là các giá trị được truyền vào hàm.

---

## 6. Hàm có nhiều tham số

Một hàm có thể có nhiều tham số.

Ví dụ:

```python
def introduce(name, age):
    print("Tên:", name)
    print("Tuổi:", age)

introduce("An", 12)
```

Kết quả:

```text
Tên: An
Tuổi: 12
```

Khi gọi hàm, các đối số được truyền theo thứ tự tương ứng với các tham số.

---

## 7. Hàm trả về giá trị

Hàm có thể trả về một kết quả bằng từ khóa `return`.

Ví dụ:

```python
def add(a, b):
    return a + b

result = add(3, 5)

print(result)
```

Kết quả:

```text
8
```

Trong ví dụ trên:

- `a` và `b` là tham số.
- `a + b` là kết quả được tính.
- `return` trả kết quả về nơi gọi hàm.
- Kết quả được lưu vào biến `result`.

---

## 8. Phân biệt `print()` và `return`

Đây là điểm quan trọng khi học hàm.

### Sử dụng `print()`

```python
def add(a, b):
    print(a + b)

add(3, 5)
```

Hàm chỉ hiển thị kết quả.

### Sử dụng `return`

```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)
```

Hàm trả kết quả để chương trình có thể tiếp tục sử dụng.

Ví dụ:

```python
def add(a, b):
    return a + b

result = add(3, 5)

new_result = result * 2

print(new_result)
```

Kết quả:

```text
16
```

---

## 9. Hàm không có tham số và không trả về

Ví dụ:

```python
def show_message():
    print("Chào mừng bạn đến với Python!")

show_message()
```

Hàm này không nhận dữ liệu và không sử dụng `return`.

---

## 10. Hàm có tham số và trả về giá trị

Đây là dạng hàm rất thường gặp.

Ví dụ:

```python
def multiply(a, b):
    return a * b

result = multiply(4, 5)

print(result)
```

Kết quả:

```text
20
```

---

## 11. Tham số mặc định

Có thể cung cấp giá trị mặc định cho tham số.

Ví dụ:

```python
def greet(name="Bạn"):
    print("Xin chào", name)

greet()
greet("An")
```

Kết quả:

```text
Xin chào Bạn
Xin chào An
```

Nếu khi gọi hàm không truyền giá trị cho `name`, Python sử dụng giá trị mặc định `"Bạn"`.

---

## 12. Hàm kết hợp với điều kiện

Có thể sử dụng `if` bên trong hàm.

Ví dụ:

```python
def check_age(age):
    if age >= 18:
        return "Đủ tuổi"
    else:
        return "Chưa đủ tuổi"

result = check_age(15)

print(result)
```

Kết quả:

```text
Chưa đủ tuổi
```

---

## 13. Hàm kết hợp với vòng lặp

Hàm cũng có thể chứa vòng lặp.

Ví dụ:

```python
def print_numbers(n):
    for i in range(1, n + 1):
        print(i)

print_numbers(5)
```

Kết quả:

```text
1
2
3
4
5
```

---

## 14. Phạm vi biến cơ bản

Biến được tạo bên trong hàm thường được sử dụng trong phạm vi của hàm đó.

Ví dụ:

```python
def calculate():
    result = 10 + 5
    print(result)

calculate()
```

Biến `result` được tạo bên trong hàm và được sử dụng trong hàm.

Khi mới học Python, nên ưu tiên truyền dữ liệu vào hàm bằng tham số và lấy kết quả bằng `return`.

---

## 15. Thực hành

### Bài tập 1

Tạo hàm:

```python
say_hello()
```

Hàm hiển thị:

```text
Hello Python!
```

---

### Bài tập 2

Tạo hàm nhận vào một tên và hiển thị lời chào.

Ví dụ:

```python
greet("An")
```

Kết quả:

```text
Xin chào An
```

---

### Bài tập 3

Tạo hàm `add(a, b)` trả về tổng của hai số.

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

### Bài tập 4

Tạo hàm `square(number)` trả về bình phương của một số.

Ví dụ:

```python
print(square(5))
```

Kết quả:

```text
25
```

---

### Bài tập 5

Tạo hàm `is_even(number)` để kiểm tra một số có phải số chẵn hay không.

Ví dụ:

```python
print(is_even(10))
```

Kết quả:

```text
True
```

---

## 16. Bài tập thử thách

### Bài tập 6: Tính điểm trung bình

Tạo hàm:

```python
calculate_average(math, physics, english)
```

Hàm nhận điểm của ba môn và trả về điểm trung bình.

Ví dụ:

```python
average = calculate_average(8, 7, 9)

print(average)
```

---

### Bài tập 7: Kiểm tra kết quả

Tạo hàm:

```python
check_result(score)
```

Quy ước:

- Điểm từ 5 trở lên → trả về `"Đạt"`.
- Điểm dưới 5 → trả về `"Chưa đạt"`.

---

### Bài tập 8: Tìm số lớn hơn

Tạo hàm nhận hai số và trả về số lớn hơn.

Ví dụ:

```python
print(max_number(10, 20))
```

Kết quả:

```text
20
```

---

## 17. Bài tập ứng dụng

Viết chương trình quản lý thông tin học sinh bằng các hàm.

Chương trình có thể gồm:

```python
def show_student(name, age, score):
    ...

def check_result(score):
    ...

def calculate_average(math, physics, english):
    ...
```

Sau đó gọi các hàm để hiển thị thông tin và kết quả học tập.

Mục tiêu là chia chương trình thành nhiều hàm nhỏ, mỗi hàm thực hiện một nhiệm vụ cụ thể.

---

## 18. Kiến thức cần nhớ

| Nội dung | Ghi nhớ |
|---|---|
| `def` | Định nghĩa một hàm |
| Gọi hàm | Sử dụng tên hàm kèm `()` |
| Tham số | Dữ liệu được truyền vào hàm |
| `return` | Trả kết quả từ hàm |
| `print()` | Hiển thị dữ liệu |
| Tham số mặc định | Giá trị được sử dụng khi không truyền đối số |
| Hàm | Giúp tái sử dụng và tổ chức mã nguồn |

> **Ghi nhớ:** Một hàm nên thực hiện một nhiệm vụ rõ ràng. Khi chương trình trở nên dài, hãy tìm những phần công việc có thể tách thành các hàm riêng.

---

## 19. Tổng kết

Trong bài học này, chúng ta đã tìm hiểu:

```text
Định nghĩa hàm
      ↓
Gọi hàm
      ↓
Truyền tham số
      ↓
Trả về kết quả
      ↓
Kết hợp hàm với if và vòng lặp
      ↓
Chia chương trình thành các chức năng nhỏ
```

Hàm là một trong những kiến thức quan trọng của Python và sẽ được sử dụng xuyên suốt các bài học tiếp theo.
