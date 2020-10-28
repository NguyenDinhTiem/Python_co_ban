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
ls = ['q', 'u', 'a', 'n', 'o', 'g']
# Xóa phần tử thứ 4 khỏi list
ls.pop(4)
print(ls)
```

    ['q', 'u', 'a', 'n', 'g']
    

> ##### **.remove()**: xoá 1 element


```python
ls = ['q', 'u', 'a', 'n', 'o', 'g']
ls.remove('o')
print(ls)
```

    ['q', 'u', 'a', 'n', 'g']
    

> ##### **.count()**: đếm phần tử cho trước


```python
ls = [0,3,9,5,0,7,7,1,9,9]
print(ls.count(9))
```

    3
    

> ##### **.reverse()**: đảo list


```python
ls = ['q', 'u', 'a', 'n', 'g']
ls.reverse()
print(ls)
```

    ['g', 'n', 'a', 'u', 'q']
    

> ##### **.sort()**: sắp xếp list


```python
ls = [0,3,9,5,0,7,7,1,9,9]
# Sort tăng dần
ls.sort()
print(ls)
# Sort giảm dần
ls.sort(reverse=True)
print(ls)
```

    [0, 0, 1, 3, 5, 7, 7, 9, 9, 9]
    [9, 9, 9, 7, 7, 5, 3, 1, 0, 0]
    

> ##### **.copy()**: copy list


```python
ls = [0,3,9,5,0,7,7,1,9,9]
ls_copy = ls.copy()
print(ls_copy)
```

    [0, 3, 9, 5, 0, 7, 7, 1, 9, 9]
    

> ##### **.clear()**: xoá toàn bộ



```python
ls = [1, 2, 3]
ls.clear()
print(ls)
```

    []
    

##### operators: +, *, so sánh


```python
ls1 = [1,2,3]
ls2 = [4,5,6]

# Nối và lặp list sử dụng +, * 2 list
print(ls1 + ls2)
print(ls1*5)

# Các phép so sánh
print(ls1 > ls2)
print(ls1 < ls2)
print(ls1 == ls2)
```

    [1, 2, 3, 4, 5, 6]
    [1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3, 1, 2, 3]
    False
    True
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
s1 = "Một con gà xòe ra 1 cái mông"
s2 = """
À sao mà à
à thế à
"""
print(s1)
print(s2)
```

    Một con gà xòe ra 1 cái mông
    
    À sao mà à
    à thế à
    
    

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
s = "abc"
print(len(s))
```

    3
    

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
    

# **PYTHON NÂNG CAO**


### **NỘI DUNG:** 

1. Mutable and Immutable
2. Slicing
3. Data Types nâng cao
4. Lambda Expressions
5. Generator Expressions
6. List Comprehension
7. Dictionary Comprehension

### **Mutable and Immutable** 

Đây là kiến thức quan trọng cần các bạn hiểu kỹ trước khi học về slicing, tuple, set và dictionary.

Đầu tiên mọi thứ trong python đều là object từ hàm, biến, mảng v.v.., đó là một phần lý do vì sao ngôn ngữ này mềm dẻo như vậy.


##### **1.Immutable**


Phép gán giá trị của biến thành giá trị khác
</br>
Ban đầu a_number = 5
![](https://i.imgur.com/izq38aU.png)

</br>

Giờ nó đổi ý muốn lưu a_number = 6
![](https://i.imgur.com/P5eMGAL.png)

> *integer, float, string, boolean, tuple là **Immutable**.*


##### **2.Mutable**

>  *List, Dictionary, Set, Class là **Mutable**.*

***Khẩu quyết Mutable: "Động đến tao thì okie sao cũng được, còn động đến con cháu tao thì coi chừng"***
</br>

Đến đây ta lại thắc mắc, và thử đặt câu hỏi "*các phần tử trong list đều là integer, string thì sao? Vậy List là **Immutable** à - không lẽ tui nói sai*"
</br>
Hmmm... 🐧

Đây là câu hỏi 10đ. Và câu trả lời là hình ảnh dưới đây:
![](https://i.imgur.com/PiuWyFv.jpg)

a_list là một đối tượng trỏ đến *list object*(**Mutable**), và trong *list object* lại trỏ đến từng đối tượng là các **Mutable** và cuối cùng trỏ đến int instance(**Immutable**).

List là **Mutable** chính nói đến đối tượng áp cuối trỏ đến int instance. Các bạn lưu ý để tránh nhầm lẫn!



> Hiểu hơn **Mutable and Immutable** để khi thao tác với kiểu dữ liệu hoặc muốn copy data đối tượng nào đó chúng ta không còn vướng bận điều gì - nice 💯

------

### **Slice** 

Biểu diễn tập hợp [start,stop)

      slice(start=0, stop, step=1)

Tuy nhiên đối tượng Slice cũng được tạo khi sử dụng cú pháp lập chỉ mục với dấu bracket [] được ngăn cách bởi dấu : <br/>

      VD: a[start:stop:step]

> ##### **list slicing**

Đây là công cụ đầy quyền lực, nó không chỉ có công dụng để truy cập phần tử mà còn có thể:

1.   Truy cập theo kiểu forward
2.   Truy cập theo kiểu Reverse
3.   Assign hùm bà lằng
4.   Insert tuỳ ý
5.   Remove tùm lum
6.   Clone list

Tôi sẽ demo kỹ code cho các bạn xem:

    Dạng: my_list[start=0:stop=-1:steps=1]

      +---+---+---+---+---+---+
      | P | y | t | h | o | n |
      +---+---+---+---+---+---+
        0   1   2   3   4   5 
       -6  -5  -4  -3  -2  -1

    index begin: 0, -length
    index end: -1, length - 1







```python
mylist = ['p','y','t','h','o','n']
n = len(mylist)
 
print("------   1. all forward  ------")
print(mylist)
print(mylist[:]) 
print(mylist[0:n])
print(mylist[-n:])
print(mylist[-n:n])

print("\n------   2. Reverse  ---------")
print(mylist[::-1]) # Recommend
print(mylist[-1:-(n + 1):-1])
print(mylist[-1::-1])
print(mylist[n-1:-(n + 1):-1])

print("\n------   3. Assign hùm bà lằng  ---------")
mylist[1:3] = [1,2,3,5]
print(mylist)

# Reset
mylist = ['p','y','t','h','o','n']

print("\n------   4. Insert tuỳ ý  ---------")
# chèn [1,2,3] vào vị trí 1
mylist[1:1] = [1,2,3]
print(mylist)

# Reset
mylist = ['p','y','t','h','o','n']

print("\n------   5. Remove tùm lum  ---------")
# Xoá từ 1 -> 2
mylist[1:3] = []
print(mylist)

# Reset
mylist = ['p','y','t','h','o','n']

print("\n------   6. Clone list  ---------")
listcopy_1 = mylist[0:3]
listcopy_2 = mylist[:] # copy toàn bộ
listcopy_1[0] = [1,2,3]
listcopy_2[0] = []
print(mylist)

```

    ------   1. all forward  ------
    ['p', 'y', 't', 'h', 'o', 'n']
    ['p', 'y', 't', 'h', 'o', 'n']
    ['p', 'y', 't', 'h', 'o', 'n']
    ['p', 'y', 't', 'h', 'o', 'n']
    ['p', 'y', 't', 'h', 'o', 'n']
    
    ------   2. Reverse  ---------
    ['n', 'o', 'h', 't', 'y', 'p']
    ['n', 'o', 'h', 't', 'y', 'p']
    ['n', 'o', 'h', 't', 'y', 'p']
    ['n', 'o', 'h', 't', 'y', 'p']
    
    ------   3. Assign hùm bà lằng  ---------
    ['p', 1, 2, 3, 5, 'h', 'o', 'n']
    
    ------   4. Insert tuỳ ý  ---------
    ['p', 1, 2, 3, 'y', 't', 'h', 'o', 'n']
    
    ------   5. Remove tùm lum  ---------
    ['p', 'h', 'o', 'n']
    
    ------   6. Clone list  ---------
    ['p', 'y', 't', 'h', 'o', 'n']
    

Nắm được slicing trong list làm ta trở nên tự tin trong việc xử lý.
Tuy nhiên sau khi đọc kỹ code ở trên thì nhiều bạn thắc mắc:
> *Tại sao listcopy_1 và listcopy_2 thay đổi hùm bà lằng nhưng mylist của ta vẫn bình yên vô sự?*

Đây là câu hỏi 10 điểm - nice 💯

Khi thực thi ***new_List = old_List*** thì new_List và old_List đang tham chiếu đến vùng nhớ. Và nếu các vùng nhớ đó là các immutable thì ta đã **sao chép thực sự**. Còn nếu vùng nhớ đó là 1 mutable thì ta phải chấp nhận là ta **chưa sao chép thực sự**. Ở đây list chứa các string hoặc int thì nó đang **sao chép thực sự**

> Bạn đọc thêm immutable và mutable ở phần ***python nâng cao***



```python
mylist = [1, [1,2,3], 4]

ok = mylist[1]
ok1 = mylist[1]
ok2 = mylist[0]
ok = [7,8,9]
ok1[1] = 34
ok2 = 100
print(mylist)
print(ok)
print(ok1)
print(ok2)
```

    [1, [1, 34, 3], 4]
    [7, 8, 9]
    [1, 34, 3]
    100
    

> ##### **Numpy slicing**

Nhiều bạn cứ ngỡ trong numpy sử dụng slicing giống như list.
Hãy đón xem tập tiếp theo ở phần numpy nhé...

------

### Các kiểu dữ liệu nâng cao

Tổng quan về kiểu dữ liệu trong python

![](https://i.imgur.com/UVw74RV.png)


    list []
    tuple ()
    set, dictionary {}

#### **Tuple** 

***Khẩu quyết tuple: "tuple là constant list"***

Dừng ở đây chắc có người chặn đường quá, haha 😂 
<br/>
<br/>
Các bạn lưu ý ở tuple các vấn đề sau:

1.   bỏ (), python vẫn hiểu đây là một tuples 

```python
tuple = "Mãi bên nhau bạn nhớ", "ok bạn ơi", 2 , 4
```

2.   Trường hợp tuples chỉ có 1 phần tử thì bên sau phần tử đó phải có dấu phẩy ',' . Nếu không nó sẽ hiểu đây là một kiểu int.


```python
tuple = (2, ) # type tuples
tuple = (2) # type int
```








### **Lambda Expressions**

> Nó là một hàm bình thường nhưng **ko cần tên hàm**, **ko cần từ khoá return** để trả về giá trị, giá trị trả về true hoặc false. 





```python
print((lambda x : x % 2 == 0) (2))
```

    True
    

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
