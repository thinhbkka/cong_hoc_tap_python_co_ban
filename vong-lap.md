# Vòng lặp trong Python

## 1. Mục tiêu bài học

Sau bài học này, người học có thể:

- Hiểu vòng lặp là gì và tại sao cần sử dụng vòng lặp.
- Biết cách sử dụng vòng lặp `for`.
- Biết cách sử dụng hàm `range()`.
- Biết cách sử dụng vòng lặp `while`.
- Hiểu cách kiểm soát vòng lặp bằng `break` và `continue`.
- Vận dụng vòng lặp để giải quyết các bài toán đơn giản.

---

## 2. Vòng lặp là gì?

Trong lập trình, có những công việc cần thực hiện nhiều lần.

Ví dụ:

- In một dòng chữ nhiều lần.
- Tính tổng nhiều số.
- Duyệt qua các phần tử trong một danh sách.
- Thực hiện một hành động cho đến khi một điều kiện không còn đúng.

Thay vì viết lại cùng một câu lệnh nhiều lần, chúng ta có thể sử dụng **vòng lặp**.

Python có hai loại vòng lặp cơ bản:

```text
for
while
```

---

## 3. Vòng lặp `for`

Vòng lặp `for` thường được sử dụng khi muốn lặp qua một tập hợp giá trị hoặc thực hiện một câu lệnh với số lần xác định.

Cú pháp:

```python
for bien in tap_hop:
    cau_lenh
```

Ví dụ:

```python
for i in range(5):
    print(i)
```

Kết quả:

```text
0
1
2
3
4
```

---

## 4. Hàm `range()`

`range()` thường được sử dụng kết hợp với vòng lặp `for`.

### 4.1. `range(stop)`

```python
for i in range(5):
    print(i)
```

Kết quả:

```text
0
1
2
3
4
```

Lưu ý: giá trị `5` không được đưa vào kết quả.

---

### 4.2. `range(start, stop)`

Có thể xác định giá trị bắt đầu:

```python
for i in range(2, 6):
    print(i)
```

Kết quả:

```text
2
3
4
5
```

---

### 4.3. `range(start, stop, step)`

Có thể xác định bước tăng:

```python
for i in range(0, 10, 2):
    print(i)
```

Kết quả:

```text
0
2
4
6
8
```

---

## 5. Ví dụ sử dụng `for`

### In một câu nhiều lần

```python
for i in range(3):
    print("Hello Python")
```

Kết quả:

```text
Hello Python
Hello Python
Hello Python
```

### Tính tổng từ 1 đến 5

```python
total = 0

for i in range(1, 6):
    total = total + i

print(total)
```

Kết quả:

```text
15
```

---

## 6. Duyệt chuỗi bằng `for`

Vòng lặp `for` có thể được sử dụng để duyệt từng ký tự trong chuỗi.

```python
name = "Python"

for character in name:
    print(character)
```

Kết quả:

```text
P
y
t
h
o
n
```

---

## 7. Vòng lặp `while`

Vòng lặp `while` được sử dụng để lặp lại câu lệnh **khi điều kiện còn đúng**.

Cú pháp:

```python
while dieu_kien:
    cau_lenh
```

Ví dụ:

```python
count = 1

while count <= 5:
    print(count)
    count = count + 1
```

Kết quả:

```text
1
2
3
4
5
```

Trong ví dụ trên:

1. `count` bắt đầu bằng `1`.
2. Python kiểm tra `count <= 5`.
3. Nếu điều kiện đúng, chương trình thực hiện câu lệnh trong vòng lặp.
4. `count` tăng lên 1.
5. Quá trình tiếp tục cho đến khi điều kiện sai.

---

## 8. Tránh vòng lặp vô hạn

Cần đảm bảo điều kiện của `while` có thể trở thành `False`.

Ví dụ:

```python
count = 1

while count <= 5:
    print(count)
    count = count + 1
```

Nếu quên cập nhật `count`:

```python
count = 1

while count <= 5:
    print(count)
```

vòng lặp có thể chạy mãi vì `count` luôn bằng `1`.

---

## 9. So sánh `for` và `while`

| `for` | `while` |
|---|---|
| Thường dùng khi biết số lần lặp hoặc cần duyệt qua tập hợp | Thường dùng khi số lần lặp phụ thuộc vào điều kiện |
| Thường kết hợp với `range()` | Dựa trên một điều kiện |
| Cú pháp ngắn gọn | Cần chú ý cập nhật biến điều kiện |
| Phù hợp để duyệt dữ liệu | Phù hợp với các tình huống lặp đến khi đạt điều kiện |

Ví dụ:

```python
for i in range(5):
    print(i)
```

và:

```python
i = 0

while i < 5:
    print(i)
    i += 1
```

Hai chương trình trên đều in:

```text
0
1
2
3
4
```

---

## 10. Câu lệnh `break`

`break` dùng để **thoát khỏi vòng lặp ngay lập tức**.

Ví dụ:

```python
for i in range(10):
    if i == 5:
        break

    print(i)
```

Kết quả:

```text
0
1
2
3
4
```

Khi `i == 5`, lệnh `break` được thực hiện và vòng lặp kết thúc.

---

## 11. Câu lệnh `continue`

`continue` dùng để **bỏ qua phần còn lại của lần lặp hiện tại** và chuyển sang lần lặp tiếp theo.

Ví dụ:

```python
for i in range(5):
    if i == 2:
        continue

    print(i)
```

Kết quả:

```text
0
1
3
4
```

Khi `i == 2`, chương trình bỏ qua lệnh `print(i)` và tiếp tục với lần lặp tiếp theo.

---

## 12. Vòng lặp kết hợp với điều kiện

Có thể sử dụng `if` bên trong vòng lặp.

Ví dụ in các số chẵn từ 1 đến 10:

```python
for i in range(1, 11):
    if i % 2 == 0:
        print(i)
```

Kết quả:

```text
2
4
6
8
10
```

---

## 13. Vòng lặp lồng nhau

Một vòng lặp có thể nằm bên trong một vòng lặp khác.

Ví dụ:

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

Kết quả:

```text
0 0
0 1
1 0
1 1
2 0
2 1
```

Vòng lặp lồng nhau thường được sử dụng khi xử lý dữ liệu có nhiều chiều hoặc các bài toán dạng bảng.

---

## 14. Thực hành

### Bài tập 1

Sử dụng `for` để in các số từ `1` đến `10`.

---

### Bài tập 2

Sử dụng `for` để in các số chẵn từ `2` đến `20`.

---

### Bài tập 3

Sử dụng `while` để in các số từ `1` đến `5`.

---

### Bài tập 4

Tính tổng các số từ `1` đến `100`.

Gợi ý:

```python
total = 0

for i in range(1, 101):
    total = total + i

print(total)
```

---

### Bài tập 5

In bảng cửu chương của số `5`.

Kết quả mong muốn:

```text
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
...
5 x 10 = 50
```

---

## 15. Bài tập thử thách

### Bài tập 6: Đếm số chẵn

Cho:

```python
numbers = [1, 4, 7, 8, 10, 13, 16]
```

Sử dụng vòng lặp để đếm có bao nhiêu số chẵn.

---

### Bài tập 7: Tìm số lớn nhất

Cho:

```python
numbers = [5, 12, 3, 20, 8]
```

Sử dụng vòng lặp để tìm số lớn nhất trong danh sách.

---

### Bài tập 8: Kiểm tra số nguyên tố

Cho một số nguyên:

```python
number = 17
```

Sử dụng vòng lặp để kiểm tra xem số đó có phải là số nguyên tố hay không.

---

## 16. Bài tập ứng dụng

Viết chương trình mô phỏng việc nhập mật khẩu.

Chương trình cho phép người dùng nhập mật khẩu tối đa 3 lần.

Ví dụ:

```text
Nhập mật khẩu: 123
Sai mật khẩu.
Nhập mật khẩu: abc
Sai mật khẩu.
Nhập mật khẩu: python123
Đăng nhập thành công.
```

Gợi ý: có thể sử dụng vòng lặp `while` kết hợp với `if`.

---

## 17. Kiến thức cần nhớ

| Nội dung | Ghi nhớ |
|---|---|
| `for` | Lặp qua tập hợp hoặc thực hiện số lần xác định |
| `while` | Lặp khi điều kiện còn đúng |
| `range()` | Tạo dãy số thường dùng với `for` |
| `break` | Thoát khỏi vòng lặp |
| `continue` | Bỏ qua lần lặp hiện tại |
| Vòng lặp lồng nhau | Một vòng lặp nằm bên trong vòng lặp khác |
| `if` trong vòng lặp | Dùng để kiểm tra điều kiện ở mỗi lần lặp |

> **Ghi nhớ:** Khi sử dụng vòng lặp `while`, luôn kiểm tra xem biến điều kiện có được cập nhật hay không để tránh vòng lặp vô hạn.
