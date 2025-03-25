# آموزش جامع NumPy برای مبتدیان

## مقدمه
NumPy (نامپای) یکی از مهم‌ترین کتابخانه‌های پایتون برای **محاسبات عددی و پردازش داده‌ها** است.
این کتابخانه مخصوص کار با **آرایه‌های چندبعدی** و عملیات ریاضی پیچیده طراحی شده است.

---

## نصب NumPy

برای استفاده از NumPy، ابتدا باید آن را نصب کنیم:

```
pip install numpy
```

سپس می‌توانیم آن را در پایتون وارد کنیم:

```python
import numpy as np
print(np.__version__)  # نمایش نسخه نصب شده
```

---

## 1. ایجاد آرایه‌ها (Array)

### 1.1 آرایه یک‌بعدی
```python
import numpy as np
arr = np.array([1, 2, 3, 4, 5])
print(arr)
```

### 1.2 آرایه دو‌بعدی (ماتریس)
```python
arr_2d = np.array([[1, 2, 3], [4, 5, 6]])
print(arr_2d)
```

### 1.3 آرایه سه‌بعدی
```python
arr_3d = np.array([[[1, 2], [3, 4]], [[5, 6], [7, 8]]])
print(arr_3d)
```

---

## 2. ویژگی‌های آرایه‌ها

### 2.1 شکل (Shape)
```python
print(arr_2d.shape)
```

### 2.2 تعداد ابعاد (ndim)
```python
print(arr.ndim)
print(arr_2d.ndim)
```

### 2.3 اندازه (size)
```python
print(arr_2d.size)
```

### 2.4 نوع داده (dtype)
```python
print(arr.dtype)
```

---

## 3. ساخت آرایه‌های خاص

### 3.1 آرایه‌ای پر از صفر
```python
zeros = np.zeros((3, 3))
print(zeros)
```

### 3.2 آرایه‌ای پر از یک
```python
ones = np.ones((2, 4))
print(ones)
```

### 3.3 آرایه تصادفی
```python
rand = np.random.rand(3, 3)
print(rand)
```

### 3.4 آرایه عددهای متوالی
```python
arange = np.arange(1, 10, 2)
print(arange)
```

---

## 4. عملیات ریاضی روی آرایه‌ها

### 4.1 جمع، تفریق، ضرب و تقسیم
```python
a = np.array([1, 2, 3])
b = np.array([4, 5, 6])
print(a + b)
print(a - b)
print(a * b)
print(a / b)
```

### 4.2 محاسبات آماری
```python
arr = np.array([10, 20, 30, 40])
print(np.sum(arr))
print(np.min(arr))
print(np.max(arr))
print(np.mean(arr))
```

---

## 5. ماتریس‌ها و جبر خطی
### 5.1 ضرب ماتریسی
```python
A = np.array([[1, 2], [3, 4]])
B = np.array([[5, 6], [7, 8]])
result = np.dot(A, B)
print(result)
```

### 5.2 ترانهاده (Transpose)
```python
print(A.T)
```

### 5.3 دترمینان ماتریس
```python
from numpy.linalg import det
print(det(A))
```

### 5.4 معکوس ماتریس
```python
from numpy.linalg import inv
print(inv(A))
```

---

## 6. چرا NumPy در یادگیری ماشین مهم است؟

✅ پردازش داده‌ها را سریع‌تر و بهینه‌تر می‌کند.✅ بسیاری از کتابخانه‌های یادگیری ماشین (مثل TensorFlow و Scikit-Learn) از NumPy استفاده می‌کنند.✅ انجام محاسبات ریاضی پیچیده مانند جبر خطی، آمار و احتمالات را ساده می‌کند.
---

## نتیجه‌گیری
نامپای یکی از **مهم‌ترین ابزارهای پردازش داده** در پایتون است.
اگر قصد یادگیری **یادگیری ماشین** را دارید، حتماً باید NumPy را **خوب یاد بگیرید** و تمرین کنید.

🎯 **تمرین پیشنهادی**: یک مجموعه داده را با NumPy پردازش کنید و عملیات ریاضی مختلف روی آن انجام دهید.
