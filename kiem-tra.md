# Kiểm tra Python cơ bản

## 1. Mục tiêu

Bài kiểm tra tổng kết giúp đánh giá mức độ nắm vững các kiến thức:

- Làm quen với Python
- Biến và kiểu dữ liệu
- Cấu trúc điều kiện
- Vòng lặp
- Hàm

---

# Phần 1. Trắc nghiệm

### Câu 1
Python là gì?

A. Một hệ điều hành  
B. Một ngôn ngữ lập trình  
C. Một phần mềm diệt virus  
D. Một cơ sở dữ liệu  

### Câu 2
Lệnh nào dùng để hiển thị dữ liệu ra màn hình?

A. `input()`  
B. `print()`  
C. `show()`  
D. `display()`

### Câu 3
Kiểu dữ liệu của giá trị `25` là:

A. `float`  
B. `str`  
C. `int`  
D. `bool`

### Câu 4
Kiểu dữ liệu của `"Python"` là:

A. `int`  
B. `float`  
C. `str`  
D. `bool`

### Câu 5
Kết quả của:

```python
x = 10
y = 3
print(x > y)
```

A. `10`  
B. `3`  
C. `True`  
D. `False`

### Câu 6
Từ khóa nào được sử dụng để tạo điều kiện?

A. `for`  
B. `if`  
C. `def`  
D. `return`

### Câu 7
Vòng lặp nào thường được sử dụng khi biết trước số lần lặp?

A. `if`  
B. `while`  
C. `for`  
D. `def`

### Câu 8
Kết quả của:

```python
for i in range(3):
    print(i)
```

là:

A.
```text
1
2
3
```

B.
```text
0
1
2
```

C.
```text
0
1
2
3
```

D.
```text
3
```

### Câu 9
Từ khóa nào dùng để định nghĩa một hàm?

A. `function`  
B. `func`  
C. `def`  
D. `define`

### Câu 10
Từ khóa `return` dùng để:

A. In dữ liệu ra màn hình  
B. Nhập dữ liệu  
C. Trả về kết quả từ hàm  
D. Tạo biến

---

# Phần 2. Đọc và dự đoán kết quả

### Câu 11

Cho chương trình:

```python
name = "An"
age = 12

print(name)
print(age)
```

Hãy cho biết kết quả chương trình.

### Câu 12

Cho chương trình:

```python
score = 8

if score >= 5:
    print("Dat")
else:
    print("Khong dat")
```

Chương trình in ra gì?

### Câu 13

Cho chương trình:

```python
for i in range(1, 6):
    print(i)
```

Có bao nhiêu số được in ra?

### Câu 14

Cho chương trình:

```python
x = 10

if x % 2 == 0:
    print("Chan")
else:
    print("Le")
```

Chương trình in ra gì?

### Câu 15

Cho chương trình:

```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)
```

Kết quả là bao nhiêu?

---

# Phần 3. Viết chương trình

### Câu 16. Thông tin cá nhân

Viết chương trình:

- Tạo biến `name`
- Tạo biến `age`
- Tạo biến `school`
- In các thông tin ra màn hình.

Ví dụ:

```text
Ho ten: An
Tuoi: 12
Truong: ABC
```

### Câu 17. Kiểm tra số chẵn lẻ

Nhập một số nguyên từ bàn phím.

Nếu số đó là số chẵn, in:

```text
So chan
```

Nếu là số lẻ, in:

```text
So le
```

### Câu 18. Xếp loại điểm

Nhập điểm của học sinh.

Quy tắc:

- Điểm >= 8: `Gioi`
- Điểm >= 6.5: `Kha`
- Điểm >= 5: `Trung binh`
- Điểm < 5: `Yeu`

### Câu 19. Tính tổng

Viết chương trình nhập số `n`.

Tính tổng:

```text
1 + 2 + 3 + ... + n
```

Ví dụ:

```text
Nhap n: 5
Tong = 15
```

### Câu 20. Hàm tính diện tích

Viết hàm:

```python
def rectangle_area(length, width):
    ...
```

Hàm nhận chiều dài và chiều rộng, sau đó trả về diện tích hình chữ nhật.

---

# Phần 4. Bài tập tổng hợp

## Câu 21. Quản lý điểm học sinh

Viết chương trình thực hiện:

1. Nhập tên học sinh.
2. Nhập điểm Toán.
3. Nhập điểm Văn.
4. Tính điểm trung bình.
5. Xếp loại học sinh.
6. In kết quả.

Ví dụ:

```text
Ho ten: An
Diem Toan: 8
Diem Van: 7

Diem trung binh: 7.5
Xep loai: Kha
```

## Câu 22. Máy tính đơn giản

Viết chương trình cho phép người dùng:

1. Nhập số thứ nhất.
2. Nhập số thứ hai.
3. Chọn phép tính:
   - `+`
   - `-`
   - `*`
   - `/`
4. Hiển thị kết quả.

## Câu 23. Trò chơi đoán số

Tạo một số bí mật.

Người chơi nhập số dự đoán.

Chương trình thông báo:

- `Lon hon` nếu số đoán nhỏ hơn số bí mật.
- `Nho hon` nếu số đoán lớn hơn số bí mật.
- `Chinh xac` nếu đoán đúng.

Sử dụng vòng lặp để cho phép người chơi đoán nhiều lần.

---

# Phần 5. Thử thách

### Câu 24. Kiểm tra số nguyên tố

Viết chương trình nhập số nguyên `n` và kiểm tra xem `n` có phải số nguyên tố hay không.

Ví dụ:

```text
Nhap n: 7
7 la so nguyen to
```

### Câu 25. Tìm số lớn nhất

Viết hàm:

```python
def find_max(a, b, c):
    ...
```

Hàm trả về số lớn nhất trong ba số `a`, `b`, `c`.

---

# Checklist trước khi nộp

- [ ] Biết sử dụng `print()`
- [ ] Biết tạo và sử dụng biến
- [ ] Phân biệt `int`, `float`, `str`, `bool`
- [ ] Biết sử dụng `if`, `elif`, `else`
- [ ] Biết sử dụng `for`
- [ ] Biết sử dụng `while`
- [ ] Biết sử dụng `break`, `continue`
- [ ] Biết tạo hàm bằng `def`
- [ ] Biết sử dụng tham số
- [ ] Biết sử dụng `return`
- [ ] Có thể kết hợp nhiều kiến thức để giải quyết một bài toán
