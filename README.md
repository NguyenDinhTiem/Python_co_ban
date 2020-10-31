## **INTRODUCTION**
Mùa thu này, khi tham gia khóa học AI Foundation Course mình học được một ngôn ngữ lập trình mới là Python- COn Trăn :)). Tại thời điểm này Python là ngôn ngữ xử lí mạnh mẽ cho Data Analytics, Machine Learning, Computing Science v.v..

# **PYTHON CƠ BẢN**



### **NỘI DUNG:** 

1. Nhập xuất cơ bản
2. Toán tử
3. Rẽ nhánh if
4. Vòng lặp
5. List
6. String


---------------------

### **1.Nhập xuất cơ bản**

#### **In ra màn hình**
Tương tự như C, java... nhưng khác là không có dấu "," ở cuối câu lệnh :))

```python
print(seft, *args, sep=' ', end = '\n', file=None)
```


```python
# In dữ liệu cách nhau bởi dấu ','
print("Hello Đại Ka :))!")
```

    Hello Đại Ka :))!
    


#### **Nhập từ bàn phím**

```python
input(message)
```




```python
# Nhập số int a xuất ra màn hình tổng a + 2
a = int(input("Nhập: "))
print(a + 2)
```

    Nhập: 2
    4
    

------

### **2.Toán tử**


Toán tử trong python được liệt kê ngắn gọn ở hình dưới đây: 

![](https://i.imgur.com/T1Je9Se.png)

* VD1: Nhập 2 số nguyên a, b và in ra tổng của chúng


```python
a = int(input("Nhập a = "))
b = int(input("Nhập b = "))
print(a + b)
```

    Nhập a = 1
    Nhập b = 2
    3
    

* VD2: in ra kết quả 2 > 3


```python
print(2 > 3)
```

    False
    

------

### **3.Rẽ nhánh if**

```python
if condition:
    # Nếu condition đúng thì khối lệnh này được thực thi
elif condition2:
    # Nếu condition2 đúng thì khối lệnh này được thực thi
else:
    # còn lại
```


* VD1: Nhập tuổi. Nếu 11 <= tuổi <= 19 thì in ra "Bạn đang tuổi teen" ngược lại in ra "Hazzzz"


```python
troinang = 1
if troinang:
    print('Tôi ngủ')
else:
    print('Tôi vẫn ngủ :))')
```

    Tôi ngủ
    

* VD2: Nhập a,b,c,d in ra số lớn nhất


```python
a = int(input("Nhập a = "))
b = int(input("Nhập b = "))
c = int(input("Nhập c = "))
d = int(input("Nhập d = "))

max = a
if (b > max):
    max = b
if (c > max):
    max = c
if (d > max):
    max = d

print("max = ", max)
```

    Nhập tuổi = 3
    Nhập tuổi = 6
    Nhập tuổi = 8
    Nhập tuổi = 3
    max =  8
    

------

### **4.Vòng lặp**

Trong python, thường người ta sẽ dùng hàm sẵn có để xử lý. Ở những trường hợp số lượng data ít ta có thể dùng vòng lặp.

#### **for loop**



```python
for element in iterable:
    #khối lệnh
```
Trong đó iterable:
  *   String
  *   Tuple
  *   List
  *   Dictionary
  *   range()




#### **while loop**

```python
while condition:
    #khối lệnh
```

------

### **5.List**



> List trong Python là một kiểu dữ liệu cho phép lưu trữ nhiều kiểu dữ liệu khác





#### **Khởi tạo**
> sử dụng cặp dấu []

```python
# Tạo list lưu trữ các số nguyên
ls1 = [2, 9, 12]
# Tạo list lưu trữ các xâu ký tự
ls2 = ["Quang", "Tiem", "Dung"]
# Tạo list lưu trữ các kiểu dữ liệu khác nhau
ls3 = [7, 3.5, "ZumpZero"]
```

> list(range(begin,end,step))



```python
ls = list(range(20))
#ls = *range(20)
print(ls)
```

    [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19]
    

#### **Truy xuất phần tử**



##### sử dụng cặp dấu []


```python
# Tạo list lưu trữ các xâu ký tự
ls = ["Quang", "Tiem", "Dung"]
# Truy cập 'Tiem'
print(ls[1])
```

#### **Hàm và phương thức**

> ##### **len()**: độ dài


```python
ls = [1,2,3]
print(len(ls))

```

    3
    

> ##### **max(), min()**



```python
ls = [1, 2, 3]
print('max =', max(ls))
print('min =', min(ls))
```

> ##### **.append()**: Thêm 1 element


```python
ls = []
ls.append(1)
ls.append(2)
ls.append(3)
print(ls)

```

    [1, 2, 3]
    

> ##### **.insert()**: thêm 1 element vào vị trí


```python
ls = ['q', 'u', 'a', 'g']
# Chèn 'n' vào vị trí thứ n trong list
ls.insert(3, 'n')
print(ls)
```

    ['q', 'u', 'a', 'n', 'g']
    

> ##### **.pop()**: xóa một element tại vị trí


```python
ls = ['k', 'a', 'n', 'e', 'n', 'g','u','y','e','n']
# Xóa phần tử thứ 4 khỏi list
ls.pop(4)
print(ls)
```

    ['k', 'a', 'n', 'e', 'g', 'u', 'y', 'e', 'n']
    

> ##### **.remove()**: xoá 1 element


```python
ls = [k', 'a', 'n', 'e', 'n', 'g','u','y','e','n']
ls.remove('o')
print(ls)
```


      File "<ipython-input-2-b0eca11278c9>", line 1
        ls = [k', 'a', 'n', 'e', 'n', 'g','u','y','e','n']
               ^
    SyntaxError: invalid syntax
    


> ##### **.count()**: đếm phần tử cho trước


```python
ls = [2,3,1,0,1,9,9,9]
print(ls.count(9))
```

    3
    

> ##### **.reverse()**: đảo list


```python
ls = ['p','i','n','k','p','a','n','t','h','e','r']
ls.reverse()
print(ls)
```

    ['r', 'e', 'h', 't', 'n', 'a', 'p', 'k', 'n', 'i', 'p']
    

> ##### **.sort()**: sắp xếp list


```python
ls = [9,9,2,3,1,0,1,1]
# Sort tăng dần
ls.sort()
print(ls)
# Sort giảm dần
ls.sort(reverse=True)
print(ls)
```

    [0, 1, 1, 1, 2, 3, 9, 9]
    [9, 9, 3, 2, 1, 1, 1, 0]
    

> ##### **.copy()**: copy list


```python
ls = [1,2,3,4,2]
ls_copy = ls.copy()
print(ls_copy)
```

    [1, 2, 3, 4, 2]
    

> ##### **.clear()**: xoá toàn bộ



```python
ls = [2,3,5,0]
ls.clear()
print(ls)
```

    []
    

##### operators: +, *, so sánh


```python
ls1 = [2,3,4,5]
ls2 = [2,3,1,0]

# Nối và lặp list sử dụng +, * 2 list
print(ls1 + ls2)
print(ls1*5)

# Các phép so sánh
print(ls1 > ls2)
print(ls1 < ls2)
print(ls1 == ls2)
```

    [2, 3, 4, 5, 2, 3, 1, 0]
    [2, 3, 4, 5, 2, 3, 4, 5, 2, 3, 4, 5, 2, 3, 4, 5, 2, 3, 4, 5]
    True
    False
    False
    

> ##### list slicing

trình bày ở phần nâng cao

------

### 6.String



> Là một tập hợp các kí tự Unicode. Không giống các ngôn ngữ khác, trong python mỗi ký tự là mỗi xâu có độ dài 1

Vì hàm và phương thức của string trong python khá nhiều nên tôi tổng quan thành sơ đồ sau:

![](https://i.imgur.com/Iqc2SKl.png)



#### **Khởi tạo**
    sử dụng ' ', " " 1 chuỗi 1 dòng
    sử dụng ''' ''', """ """ 1 chuỗi nhiều dòng



```python
s1 = "Muôn kiếp nhân sinh"
s2 = """
Chiến binh cầu vồng
Hai số phận
Không gia đình
"""
print(s1)
print(s2)
```

    Muôn kiếp nhân sinh
    
    Chiến binh cầu vồng
    Hai số phận
    Không gia đình
    
    

#### **Truy xuất phần tử**


> ##### sử dụng cặp dấu []


```python
s = "A lí a a a í í í hí hí lí la"
print(s[3])

```

    í
    

#### **Hàm và phương thức**





> ##### len(): độ dài



```python
s = "Gió là những luồng không khí chuyển động trên quy mô lớn. Trên bề mặt của Trái Đất, gió bao gồm một khối không khí lớn chuyển động. Trong không gian vũ trụ, gió mặt trời là sự chuyển động của các chất khí hoặc các hạt tích điện từ Mặt Trời vào không gian, trong khi gió hành tinh là sự thoát khí của nguyên tố hóa học nhẹ chuyển từ bầu khí quyển của một hành tinh vào không gian. Gió thường được phân loại theo quy mô về không gian, tốc độ, lực tạo ra gió, các khu vực gió xảy ra, và tác động của chúng. Những cơn gió mạnh nhất được quan sát trên một hành tinh trong hệ mặt trời của chúng ta xảy ra trên sao Hải Vương và sao Thổ. Gió có những khía cạnh khác nhau, một là vận tốc của gió; hai là áp suất dòng khí; ba là tổng năng lượng của gió."
print(len(s))
```

    743
    

> ##### .lower(): chuyển 1 chuỗi về dạng in thường


```python
s = "Pink Paner"
print(s.lower())
```

    pink paner
    

> ##### .upper(): chuyển 1 chuỗi về dạng in hoa



```python
s = "Bangtan"
print(s.upper())
```

    BANGTAN
    


```python
s = "aaa"
print(s.isupper())
print("AAA".isupper())
```

    False
    True
    

> ##### .isdigit(): kiểm tra có gồm tất cả kí tự số



```python
s = "2020"
print(s.isdigit())
print("aaaaaaaaaaa".isdigit())
```

    True
    False
    

> ##### .isalpha(): kiểm tra gồm tất cả chữ cái



```python
s = "2020"
print(s.isalpha())
print("aaaaaaaaaaa".isalpha())
```

    False
    True
    

> ##### .split(): cắt chuỗi




```python
s = "Bỗng nhận ra hương ổi, phả vào trong .."
print(s.split(" "))
```

    ['Bỗng', 'nhận', 'ra', 'hương', 'ổi,', 'phả', 'vào', 'trong', '..']
    

> ##### .join(): nối chuỗi


```python
ls = ["Yêu", "em", "không", "anh", "?"]
print(" ".join(ls))

# Cắt thành list sau khi bỏ khoảng trắng và join list string lại
message = "   Con vịt     xinh đẹp   "
print(" ".join(message.split()))
```

    Yêu em không anh ?
    Con vịt xinh đẹp
    

> ##### .replace(): thay thế



```python
s = "Cạn lời"
print(s.replace(" ", "<3"))
```

    Cạn<3lời
    

> ##### eval():tính biểu thức từ chuỗi

Bạn nào học về ký pháp balan rồi chắc cảm thấy có hàm này tự nhiên trẻ ra được mấy chục tuổi vậy@@



```python
s = "(23/10)*2"

print(eval(s))
```

    4.6
    

# **BÀI TẬP**


```python
'''
Tính e = 1 + 1/1! + 1/2! + ...
'''
import math

n = 40
e = sum([1/math.factorial(i) for i in range(n)])
print(e)
```

    2.7182818284590455
    


```python
'''
Tính căn bậc 2 của N
'''

from functools import reduce
iterator = 20
N = 9
quadratic = reduce((lambda x,_: (x + N/x)/2.0), [N/2,*range(iterator)])
print(quadratic)
```

    3.0
    


```python
'''
Tính pi
'''

from random import uniform

coor = [0,0]
Nr = 1000000
Nc = sum([(uniform(-1,1)**2 + uniform(-1,1)**2 < 1) for _ in range(Nr)])

print("pi = ", 4*Nc/Nr)
            
```

    pi =  3.143816
    


```python

```

Bài viết được dựa trên tài liệu khóa học mùa thu AI Found Course in AI Viet Nam
