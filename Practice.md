


## 1. Hello, World！ 
**目标**：初步体验 Python 的运行与输出

1. 安装好 Python 或在在线环境（如 Jupyter Notebook、Repl.it）中输入以下代码：
   ```python
   print("Hello, World!")
   ```
2. 运行代码，观察结果。
3. 尝试修改输出的内容，例如输出你的名字或任何你想说的话。

---

## 2. 变量与数据类型
**目标**：理解并使用变量，以及熟悉 Python 中常见的数据类型

1. 定义不同类型的变量，例如：
   - 整数（`int`）
   - 浮点数（`float`）
   - 字符串（`str`）
   - 布尔值（`bool`）
2. 使用 `type()` 函数查看变量类型：
   ```python
   my_int = 10
   my_float = 3.14
   my_str = "Python"
   my_bool = True
   ```
3. 将不同类型的变量输出在屏幕上。

---

## 3. 运算与格式化输出
**目标**：掌握 Python 中的算术运算以及简单的字符串格式化

1. 使用加（+）、减（-）、乘（*）、除（/）、整除（//）、取余（%）和幂运算（**）完成下列运算，并输出结果：  
   - 10 + 5
   - 10 - 5
   - 10 * 5
   - 10 / 3
   - 10 // 3
   - 10 % 3
   - 2 ** 3
2. 将结果打印出来，例如：
   ```python
   result1 = 10 + 5
   print(f"10 + 5 = {result1}")
   ```
3. 尝试用 `format()` 或者 f-string 做更多格式化输出练习。

---

## 4. 字符串处理
**目标**：熟悉字符串的基本操作

1. 定义一个字符串 `text = "Hello, Python!"`。
2. 尝试以下操作：
   - 访问字符串的第一个和最后一个字符
   - 使用切片 `text[start:end:step]` 截取字符串的不同部分
   - 使用内置方法：`upper()`, `lower()`, `replace()`, `split()`, `strip()` 等
3. 将每一次操作的结果打印出来。

---

## 5. 条件判断
**目标**：掌握 if-else、elif 语句的使用

1. 从键盘输入一个整数（使用 `input()` 并用 `int()` 转换）。
2. 判断这个数是正数、负数还是零，并分别输出不同的提示信息。
   ```python
   num = int(input("请输入一个整数："))
   if num > 0:
       print("这是一个正数")
   elif num < 0:
       print("这是一个负数")
   else:
       print("这是零")
   ```
3. 根据兴趣添加更多条件判断，例如判断是否为偶数、奇数等。

---

## 6. 循环
**目标**：熟悉 for 循环和 while 循环

1. 使用 `for` 循环打印从 1 到 10 的所有整数。  
2. 使用 `while` 循环计算从 1 到 100 的和。  
3. 使用循环输出一个乘法表（如 99 乘法表）。

---

## 7. 列表与元组
**目标**：学习使用列表和元组，以及常见的增删改查操作

1. 创建一个列表 `my_list = [1, 2, 3, "Python", True]`：
   - 打印列表的长度、访问某个元素
   - 使用 `append()`、`insert()`、`remove()`、`pop()` 等方法操作列表
   - 遍历列表中的每个元素并打印
2. 创建一个元组 `my_tuple = (10, 20, 30, "Hello")`：
   - 尝试修改一个元组元素，观察是否报错
   - 访问元组元素，切片元组

---

## 8. 字典与集合
**目标**：掌握字典和集合的定义及常用操作

1. 定义一个字典，包含以下信息：
   ```python
   person = {
       "name": "Alice",
       "age": 25,
       "city": "Beijing"
   }
   ```
   - 访问字典中的值，修改 age 的值，添加新的键值对
   - 使用 `items()`、`keys()`、`values()` 遍历字典
2. 定义一个集合 `my_set = {1, 2, 3, 2, 1}`，观察打印结果。
   - 向集合中添加新元素，尝试重复添加，看结果有何不同
   - 了解集合的去重特性和常用操作（如 `union()`、`intersection()` 等）

---

## 9. 函数基础
**目标**：学会定义和调用函数

1. 定义一个函数 `greet(name)`，传入一个名字并在函数中打印问候语。
   ```python
   def greet(name):
       print(f"Hello, {name}!")
   ```
   - 调用 `greet("Alice")`, 观察输出结果
2. 定义一个函数 `add(a, b)` 返回两个数的和，分别传入不同的实参进行测试。
3. 定义一个函数 `factorial(n)`，用循环或递归方法计算 `n` 的阶乘，并返回结果。

---

## 10. 递归函数
**目标**：理解递归的概念与用法

1. 用递归实现求阶乘函数 `factorial(n)`。
2. 使用递归实现斐波那契数列（Fibonacci）第 `n` 项的计算：
   ```python
   def fibonacci(n):
       if n <= 1:
           return n
       else:
           return fibonacci(n - 1) + fibonacci(n - 2)
   ```
3. 注意递归层数过深时可能会引发错误，了解 `sys.setrecursionlimit()` 的作用。

---

## 11. 文件读写
**目标**：学会使用 Python 进行简单的文件读写操作

1. 新建一个文本文件 `data.txt`，写入几行自己喜欢的文字。
2. 使用以下代码读取文件内容并打印：
   ```python
   with open("data.txt", "r", encoding="utf-8") as f:
       content = f.read()
       print(content)
   ```
3. 用追加模式写入一行新的文字，然后再次读取文件，打印新内容。

---

## 12. 异常处理
**目标**：掌握 try-except 结构，处理程序运行中的异常

1. 在一个函数中尝试做除法操作，让用户从键盘输入被除数和除数：
   ```python
   def divide():
       try:
           a = int(input("请输入被除数："))
           b = int(input("请输入除数："))
           result = a / b
           print(f"结果是：{result}")
       except ZeroDivisionError:
           print("错误：除数不能为零！")
       except ValueError:
           print("错误：请输入正确的整数！")
   ```
2. 测试不同的输入场景，看程序如何处理异常。

---

## 13. 自定义模块
**目标**：了解 Python 模块的概念，并使用自定义模块

1. 新建一个脚本文件 `mymodule.py`，定义如下函数：
   ```python
   def say_hello(name):
       print(f"Hello, {name}!")
   ```
2. 在另一脚本 `main.py` 中导入该模块并调用函数：
   ```python
   import mymodule

   mymodule.say_hello("Alice")
   ```
3. 进一步尝试使用 `from mymodule import say_hello` 等不同的导入方式。

---

## 14. 类与对象 (面向对象入门)
**目标**：学习如何定义类、创建对象以及访问属性和方法

1. 定义一个类 `Person`，包含以下内容：
   - 构造函数 `__init__`，接受 `name` 和 `age` 两个参数，并将其保存在实例属性中
   - 一个方法 `introduce()`，打印姓名和年龄
   ```python
   class Person:
       def __init__(self, name, age):
           self.name = name
           self.age = age

       def introduce(self):
           print(f"大家好，我是{self.name}，今年{self.age}岁。")
   ```
2. 创建 `Person` 类的实例并调用 `introduce()` 方法：
   ```python
   p1 = Person("Alice", 25)
   p1.introduce()
   ```
3. 尝试给 `Person` 类添加更多属性或方法，例如记录地址、性别，或定义 `birthday()` 方法让年龄加一等。

---

## 15. 继承与多态（进阶）
**目标**：深入理解面向对象的继承、多态特性

1. 定义一个父类 `Animal`：
   - 包含 `name` 属性和 `speak()` 方法
2. 定义两个子类 `Dog` 和 `Cat`，继承自 `Animal`：
   ```python
   class Animal:
       def __init__(self, name):
           self.name = name

       def speak(self):
           print("Some generic animal sound")

   class Dog(Animal):
       def speak(self):
           print("Woof!")

   class Cat(Animal):
       def speak(self):
           print("Meow!")
   ```
3. 创建 `Dog` 和 `Cat` 的对象，并调用 `speak()` 方法，观察多态表现。
4. 在子类中添加各自专有的属性或方法，进一步体验面向对象编程。

---
