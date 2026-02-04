# BIT250327_Diep-Tu-Thanh-
#%%
#Bài 1
integer_var = 10
float_var = 3.14
string_var = "Hello Python"

print(integer_var)
print(float_var)
print(string_var)
#%%
#Bài 2
PI = 3.14
r = 5
chu_vi = 2 * PI * r

print("Chu vi hình tròn là:", chu_vi)
#%%
#Bài 3
a = int(input("Nhập số thứ nhất: "))
b = int(input("Nhập số thứ hai: "))

print("Tổng:", a + b)
print("Hiệu:", a - b)
print("Tích:", a * b)

if b != 0:
    print("Thương:", a / b)
else:
    print("Không thể chia cho 0")
#%%
#Bài 4
def sum_two_numbers(a, b):
    return a + b

result = sum_two_numbers(3, 5)
print("Tổng hai số là:", result)
#%%
#Bài 5
name = "An"
age = 18
average_score = 7.5

print(type(name))
print(type(age))
print(type(average_score))

age_next_year = age + 1
doubled_score = average_score * 2

print("Tên:", name)
print("Tuổi:", age)
print("Tuổi năm sau:", age_next_year)
print("Điểm TB:", average_score)
print("Điểm nhân đôi:", doubled_score)
#%%
#Bài 6
def is_even(n):
    return n % 2 == 0

print(is_even(4))
print(is_even(7))
#%%
#Bài 7
a = int(input("Nhập số thứ nhất: "))
b = int(input("Nhập số thứ hai: "))
c = int(input("Nhập số thứ ba: "))

print("Số lớn nhất là:", max(a, b, c))
#%%
#Bài 8
def greet(name="Student"):
    print(f"Hello, {name}!")

greet()
greet("An")
#%%
#Bài 9
age = int(input("Nhập tuổi: "))

if 1 <= age <= 120:
    print("Tuổi hợp lệ")
else:
    print("Tuổi không hợp lệ")
#%%
#Bài 10
s = input("Nhập chuỗi: ")
count = s.count('a')

print("Số lần xuất hiện của 'a':", count)
#%%
#Bài 11
c = float(input("Nhập nhiệt độ (°C): "))
f = c * 9 / 5 + 32

print(f"Nhiệt độ tương ứng là {f:.2f}°F")
#%%
#Bài 12
weight = float(input("Nhập cân nặng (kg): "))
height = float(input("Nhập chiều cao (m): "))

bmi = weight / (height * height)
print(f"BMI của bạn là: {bmi:.2f}")
#%%
#Bài 13
try:
    a = int(input("Nhập số thứ nhất: "))
    b = int(input("Nhập số thứ hai: "))
    print("Kết quả:", a / b)
except ZeroDivisionError:
    print("Lỗi: Không thể chia cho 0")
except ValueError:
    print("Lỗi: Dữ liệu nhập không hợp lệ")
#%%
#Bài 14
import math

n = float(input("Nhập một số: "))

if n < 0:
    print("Lỗi: Không thể tính căn bậc hai của số âm")
else:
    print("Căn bậc hai là:", math.sqrt(n))
#%%
#Bài 15
for i in range(1, 4):
    print(f"\nSinh viên {i}")
    name = input("Tên: ")
    toan = float(input("Điểm Toán: "))
    ly = float(input("Điểm Lý: "))
    hoa = float(input("Điểm Hóa: "))

    avg = (toan + ly + hoa) / 3
    print(f"Sinh viên {name} có điểm trung bình: {avg:.2f}")
