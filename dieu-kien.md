# Cấu trúc điều kiện trong Python

## 1. Mục tiêu bài học

Sau bài học này, người học có thể:

- Hiểu cấu trúc điều kiện trong Python.
- Biết cách sử dụng `if`.
- Biết cách sử dụng `if...else`.
- Biết cách sử dụng `if...elif...else`.
- Sử dụng điều kiện để chương trình đưa ra quyết định.
- Kết hợp điều kiện với các phép so sánh và giá trị Boolean.

---

## 2. Cấu trúc điều kiện là gì?

Trong chương trình, có nhiều trường hợp chúng ta cần thực hiện một hành động **chỉ khi một điều kiện nào đó đúng**.

Ví dụ:

- Nếu điểm lớn hơn hoặc bằng 5 → thông báo đạt.
- Nếu tuổi lớn hơn hoặc bằng 18 → thông báo đủ tuổi.
- Nếu trời mưa → mang theo ô.

Python sử dụng các từ khóa:

```python
if
elif
else
```

để xây dựng cấu trúc điều kiện.

---

## 3. Câu lệnh `if`

Câu lệnh `if` dùng để thực hiện một nhóm câu lệnh khi điều kiện đúng.

Cú pháp:

```python
if dieu_kien:
    cau_lenh
```

Ví dụ:

```python
age = 18

if age >= 18:
    print("Bạn đã đủ 18 tuổi.")
```

Kết quả:

```text
Bạn đã đủ 18 tuổi.
```

Nếu điều kiện `age >= 18` là `False`, câu lệnh `print()` sẽ không được thực hiện.

---

## 4. Thụt lề trong Python

Python sử dụng **thụt lề (indentation)** để xác định các câu lệnh thuộc một khối.

Ví dụ đúng:

```python
age = 18

if age >= 18:
    print("Đủ tuổi.")
```

Ví dụ sai:

```python
age = 18

if age >= 18:
print("Đủ tuổi.")
```

Thông thường, mỗi cấp thụt lề sử dụng **4 dấu cách**.

---

## 5. Câu lệnh `if...else`

Khi muốn chương trình xử lý **hai trường hợp**, có thể sử dụng `if...else`.

Cú pháp:

```python
if dieu_kien:
    cau_lenh_1
else:
    cau_lenh_2
```

Ví dụ:

```python
age = 15

if age >= 18:
    print("Đủ tuổi.")
else:
    print("Chưa đủ tuổi.")
```

Kết quả:

```text
Chưa đủ tuổi.
```

Nếu điều kiện đúng, chương trình thực hiện phần `if`.

Nếu điều kiện sai, chương trình thực hiện phần `else`.

---

## 6. Sử dụng điều kiện với điểm số

Ví dụ kiểm tra kết quả học tập:

```python
score = 8

if score >= 5:
    print("Đạt")
else:
    print("Chưa đạt")
```

Kết quả:

```text
Đạt
```

---

## 7. Câu lệnh `if...elif...else`

Khi có nhiều trường hợp cần kiểm tra, sử dụng `elif`.

Cú pháp:

```python
if dieu_kien_1:
    cau_lenh_1
elif dieu_kien_2:
    cau_lenh_2
else:
    cau_lenh_3
```

Ví dụ:

```python
score = 8

if score >= 9:
    print("Xuất sắc")
elif score >= 7:
    print("Tốt")
elif score >= 5:
    print("Đạt")
else:
    print("Chưa đạt")
```

Kết quả:

```text
Tốt
```

Python kiểm tra các điều kiện **từ trên xuống dưới**.

Khi gặp điều kiện đúng, Python thực hiện khối lệnh tương ứng và bỏ qua các điều kiện còn lại.

---

## 8. So sánh nhiều giá trị

Có thể sử dụng các toán tử so sánh để xây dựng điều kiện:

| Toán tử | Ý nghĩa |
|---|---|
| `==` | Bằng |
| `!=` | Khác |
| `>` | Lớn hơn |
| `<` | Nhỏ hơn |
| `>=` | Lớn hơn hoặc bằng |
| `<=` | Nhỏ hơn hoặc bằng |

Ví dụ:

```python
age = 15

if age == 15:
    print("Tuổi bằng 15.")
```

---

## 9. Kết hợp nhiều điều kiện

Có thể sử dụng các toán tử logic:

| Toán tử | Ý nghĩa |
|---|---|
| `and` | Và |
| `or` | Hoặc |
| `not` | Phủ định |

### Ví dụ với `and`

```python
age = 15
score = 8

if age >= 10 and score >= 5:
    print("Điều kiện được thỏa mãn.")
```

Cả hai điều kiện phải đúng.

### Ví dụ với `or`

```python
day = "Saturday"

if day == "Saturday" or day == "Sunday":
    print("Cuối tuần.")
```

Chỉ cần một trong hai điều kiện đúng.

### Ví dụ với `not`

```python
is_raining = False

if not is_raining:
    print("Không mưa.")
```

---

## 10. Điều kiện với Boolean

Boolean chỉ có hai giá trị:

```python
True
False
```

Có thể sử dụng trực tiếp trong điều kiện:

```python
is_student = True

if is_student:
    print("Đây là học sinh.")
```

Ví dụ với `False`:

```python
is_raining = False

if is_raining:
    print("Mang theo ô.")
else:
    print("Không cần mang ô.")
```

---

## 11. Điều kiện lồng nhau

Một câu lệnh điều kiện có thể nằm bên trong một câu lệnh điều kiện khác.

Ví dụ:

```python
age = 15
has_card = True

if age >= 12:
    if has_card:
        print("Được phép vào.")
    else:
        print("Cần có thẻ.")
else:
    print("Chưa đủ tuổi.")
```

Khi mới học, nên ưu tiên viết điều kiện rõ ràng và đơn giản trước khi sử dụng điều kiện lồng nhau.

---

## 12. Thực hành

### Bài tập 1

Cho:

```python
number = 10
```

Kiểm tra xem `number` có lớn hơn 5 hay không.

---

### Bài tập 2

Cho:

```python
age = 16
```

Viết chương trình kiểm tra:

- Nếu tuổi từ 18 trở lên → in `Đủ tuổi`.
- Nếu nhỏ hơn 18 → in `Chưa đủ tuổi`.

---

### Bài tập 3

Cho:

```python
score = 7.5
```

Phân loại kết quả:

- Từ 9 trở lên → `Xuất sắc`
- Từ 7 đến dưới 9 → `Tốt`
- Từ 5 đến dưới 7 → `Đạt`
- Dưới 5 → `Chưa đạt`

---

### Bài tập 4

Cho:

```python
number = 12
```

Kiểm tra xem số đó có phải là số chẵn hay không.

Gợi ý:

```python
number % 2
```

---

### Bài tập 5

Cho:

```python
age = 12
score = 8
```

Kiểm tra xem người học có:

- Tuổi từ 10 trở lên.
- Điểm từ 5 trở lên.

Nếu cả hai điều kiện đều đúng, in:

```text
Đủ điều kiện.
```

---

## 13. Bài tập thử thách

Viết chương trình kiểm tra một số nguyên:

```python
number = 15
```

Chương trình cần thông báo:

- Số lớn hơn 0 → `Số dương`
- Số nhỏ hơn 0 → `Số âm`
- Số bằng 0 → `Bằng 0`

Gợi ý:

```python
if ...
elif ...
else ...
```

---

## 14. Bài tập ứng dụng

Viết chương trình kiểm tra nhiệt độ:

```python
temperature = 30
```

Quy ước:

- Từ 35°C trở lên → `Rất nóng`
- Từ 25°C đến dưới 35°C → `Nóng`
- Từ 15°C đến dưới 25°C → `Mát`
- Dưới 15°C → `Lạnh`

Chương trình cần hiển thị đúng thông báo tương ứng.

---

## 15. Kiến thức cần nhớ

| Nội dung | Ghi nhớ |
|---|---|
| `if` | Thực hiện lệnh khi điều kiện đúng |
| `else` | Xử lý trường hợp điều kiện sai |
| `elif` | Kiểm tra thêm điều kiện khác |
| `==` | So sánh bằng |
| `!=` | So sánh khác |
| `>` / `<` | Lớn hơn / nhỏ hơn |
| `>=` / `<=` | Lớn hơn hoặc bằng / nhỏ hơn hoặc bằng |
| `and` | Các điều kiện đều đúng |
| `or` | Ít nhất một điều kiện đúng |
| `not` | Phủ định điều kiện |
| Indentation | Xác định khối lệnh |

> **Ghi nhớ:** Cấu trúc điều kiện giúp chương trình có khả năng đưa ra quyết định dựa trên dữ liệu. Hãy luyện tập với nhiều giá trị khác nhau để quan sát cách chương trình thay đổi kết quả.
