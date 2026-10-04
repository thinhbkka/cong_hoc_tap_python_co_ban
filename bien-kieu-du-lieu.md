# Biến và kiểu dữ liệu

## 1. Mục tiêu bài học

Sau bài học này, người học có thể:

- Hiểu biến trong Python là gì.
- Biết cách tạo và sử dụng biến.
- Biết các kiểu dữ liệu cơ bản trong Python.
- Phân biệt số nguyên, số thực, chuỗi và Boolean.
- Biết cách kiểm tra kiểu dữ liệu bằng `type()`.
- Biết cách thay đổi giá trị của biến.

---

## 2. Biến trong Python

**Biến (variable)** là tên dùng để tham chiếu đến một giá trị được lưu trữ trong chương trình.

Ví dụ:

```python
name = "An"
age = 12
```

Trong ví dụ trên:

- `name` là biến chứa chuỗi `"An"`.
- `age` là biến chứa số `12`.

Python không yêu cầu khai báo kiểu dữ liệu trước khi sử dụng biến.

---

## 3. Tạo và gán giá trị cho biến

Cú pháp:

```python
ten_bien = gia_tri
```

Ví dụ:

```python
name = "An"
age = 12
score = 8.5
```

Có thể sử dụng biến sau khi gán:

```python
name = "An"
print(name)
```

Kết quả:

```text
An
```

---

## 4. Thay đổi giá trị của biến

Giá trị của biến có thể được thay đổi trong quá trình chương trình chạy.

```python
age = 12
print(age)

age = 13
print(age)
```

Kết quả:

```text
12
13
```

---

## 5. Các kiểu dữ liệu cơ bản

Trong Python, một số kiểu dữ liệu cơ bản thường gặp là:

| Kiểu | Tên | Ví dụ |
|---|---|---|
| `int` | Số nguyên | `10`, `-5`, `0` |
| `float` | Số thực | `3.14`, `8.5` |
| `str` | Chuỗi | `"Python"` |
| `bool` | Boolean | `True`, `False` |

---

## 6. Kiểu số nguyên `int`

`int` dùng để biểu diễn các số nguyên.

Ví dụ:

```python
age = 12
number = -5
count = 0
```

Có thể thực hiện các phép tính với số nguyên:

```python
a = 10
b = 3

print(a + b)
print(a - b)
print(a * b)
```

Kết quả:

```text
13
7
30
```

---

## 7. Kiểu số thực `float`

`float` dùng để biểu diễn các số có phần thập phân.

Ví dụ:

```python
height = 1.65
score = 8.5
temperature = 25.5
```

Có thể thực hiện phép tính với số thực:

```python
a = 10.5
b = 2.5

print(a + b)
print(a * b)
```

Kết quả:

```text
13.0
26.25
```

---

## 8. Kiểu chuỗi `str`

`str` dùng để lưu trữ văn bản hoặc một chuỗi ký tự.

Chuỗi có thể được đặt trong dấu nháy đơn hoặc dấu nháy kép:

```python
name = "An"
city = 'Da Nang'
```

Ví dụ:

```python
name = "An"
print(name)
```

Kết quả:

```text
An
```

Có thể nối các chuỗi bằng toán tử `+`:

```python
first_name = "Nguyen"
last_name = "An"

full_name = first_name + " " + last_name

print(full_name)
```

Kết quả:

```text
Nguyen An
```

---

## 9. Kiểu Boolean `bool`

`bool` chỉ có hai giá trị:

```python
True
False
```

Boolean thường được sử dụng để biểu diễn trạng thái đúng hoặc sai.

Ví dụ:

```python
is_student = True
is_teacher = False

print(is_student)
print(is_teacher)
```

Kết quả:

```text
True
False
```

Kiểu `bool` sẽ được sử dụng nhiều khi học về **cấu trúc điều kiện**.

---

## 10. Kiểm tra kiểu dữ liệu bằng `type()`

Hàm `type()` cho biết kiểu dữ liệu của một giá trị hoặc biến.

Ví dụ:

```python
age = 12
score = 8.5
name = "An"
is_student = True

print(type(age))
print(type(score))
print(type(name))
print(type(is_student))
```

Kết quả:

```text
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```

---

## 11. Một biến có thể nhận kiểu dữ liệu khác

Python cho phép một biến nhận giá trị thuộc kiểu dữ liệu khác trong quá trình chạy chương trình.

Ví dụ:

```python
data = 10
print(type(data))

data = "Python"
print(type(data))
```

Kết quả:

```text
<class 'int'>
<class 'str'>
```

Điều này thể hiện tính linh hoạt của Python.

---

## 12. Quy tắc đặt tên biến

Khi đặt tên biến, cần lưu ý:

- Tên biến có thể chứa chữ cái, chữ số và dấu gạch dưới `_`.
- Không được bắt đầu bằng chữ số.
- Không được chứa khoảng trắng.
- Không nên sử dụng từ khóa của Python làm tên biến.
- Nên đặt tên có ý nghĩa và dễ hiểu.

Ví dụ hợp lệ:

```python
name = "An"
student_age = 12
score1 = 9
```

Ví dụ không hợp lệ:

```python
1name = "An"
student age = 12
```

---

## 13. Thực hành

### Bài tập 1

Tạo ba biến:

```text
name
age
score
```

và gán lần lượt:

```text
Tên của bạn
Tuổi của bạn
Điểm của bạn
```

Sau đó sử dụng `print()` để hiển thị các giá trị.

### Bài tập 2

Tạo các biến sau:

```python
a = 10
b = 5
```

Tính và hiển thị:

- Tổng của `a` và `b`.
- Hiệu của `a` và `b`.
- Tích của `a` và `b`.

### Bài tập 3

Tạo một biến chứa tên của bạn và kiểm tra kiểu dữ liệu bằng `type()`.

### Bài tập 4

Tạo một biến Boolean:

```python
is_student = True
```

Sau đó hiển thị giá trị và kiểu dữ liệu của biến.

---

## 14. Bài tập thử thách

Viết chương trình lưu thông tin của một học sinh:

```python
name = "An"
age = 12
score = 8.5
is_student = True
```

Sau đó hiển thị thông tin theo dạng:

```text
Tên: An
Tuổi: 12
Điểm: 8.5
Là học sinh: True
```

Cuối cùng, sử dụng `type()` để kiểm tra kiểu dữ liệu của từng biến.

---

## 15. Kiến thức cần nhớ

| Nội dung | Ghi nhớ |
|---|---|
| Biến | Tên dùng để tham chiếu đến một giá trị |
| `int` | Số nguyên |
| `float` | Số thực |
| `str` | Chuỗi ký tự |
| `bool` | Đúng hoặc sai (`True` / `False`) |
| `type()` | Kiểm tra kiểu dữ liệu |
| `=` | Gán giá trị cho biến |

> **Ghi nhớ:** Hãy tự tạo biến với nhiều giá trị khác nhau và dùng `type()` để quan sát kiểu dữ liệu. Việc thực hành giúp hiểu rõ hơn cách Python xử lý dữ liệu.
