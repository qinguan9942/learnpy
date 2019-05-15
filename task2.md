
Task3（2day）
1. Dict字典
1） 定义
2） 创建
3） 字典的方法
2. 集合
1） 特性
2） 创建
3） 方法
3. 判断语句（要求掌握多条件判断）
4. 三目表达式
循环语句

#task3
##Dictus字典
###定义：
字典是一种可通过名称来访问其各个值的数据结构。这种数据结构称为映射（ mapping）。字典是Python中唯一的内置映射类型，其中的值不按顺序排列，而是存储在键下。键可能是数、字符串或元组。
###字典的创建：
可使用函数dict从其他映射（如其他字典）或键/值对序列创建字典  
>>> items = [('name', 'Gumby'), ('age', 42)]
>>> d = dict(items)
>>> d
{'age': 42, 'name': 'Gumby'}
>>> d['name']
'Gumby'  
 
还可使用关键字实参来调用这个函数，如下所示：
>>> d = dict(name='Gumby', age=42)
>>> d
{'age': 42, 'name': 'Gumby'}
  
###字典的方法：  
字典的基本行为在很多方面都类似于序列。  

len(d)返回字典d包含的项（键值对）数。 

d[k]返回与键k相关联的值。  

d[k] = v将值v关联到键k。  

del d[k]删除键为k的项。  

 k in d检查字典d是否包含键为k的项。  

虽然字典和列表有多个相同之处，但也有一些重要的不同之处。  
 键的类型：字典中的键可以是整数，但并非必须是整数。字典中的键可以是任何不可变
的类型，如浮点数（实数）、字符串或元组。  

 自动添加：即便是字典中原本没有的键，也可以给它赋值，这将在字典中创建一个新项。
然而，如果不使用append或其他类似的方法，就不能给列表中没有的元素赋值。  

 成员资格：表达式k in d（其中d是一个字典）查找的是键而不是值，而表达式v in l（其
中l是一个列表）查找的是值而不是索引。这看似不太一致，但你习惯后就会觉得相当自
然。毕竟如果字典包含指定的键，检查相应的值就很容易
##集合
###定义：  
集合（set）是一个无序的不重复元素序列。
###特性：  
集合（set）是一个无序的不重复元素序列。
###创建：  
可以使用大括号 { } 或者 set() 函数创建集合，注意：创建一个空集合必须用 set() 而不是 { }，因为 { } 是用来创建一个空字典。   

创建格式：  

     parame = {value01,value02,...}
或者  
    
    set(value)  
###基本操作：  
1、添加元素  
语法格式如下：  

    s.add( x )
将元素 x 添加到集合 s 中，如果元素已存在，则不进行任何操作。  
  
    thisset = set(("Google", "Runoob", "Taobao"))  

    thisset.add("Facebook") print(thisset)  

    {'Taobao', 'Facebook', 'Google', 'Runoob'}  
还有一个方法，也可以添加元素，且参数可以是列表，元组，字典等，语法格式如下：  
 `s.update( x )`  
2、移除元素  
语法格式如下：    
    s.remove( x )  
>>>thisset = set(("Google", "Runoob", "Taobao"))  
>
>>> thisset.remove("Taobao")  
>
>>> print(thisset)
{'Google', 'Runoob'}  

>>> thisset.remove("Facebook")   # 不存在会发生错误  
>
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>  

KeyError: 'Facebook'  


此外还有一个方法也是移除集合中的元素，且如果元素不存在，不会发生错误。格式如下所示：  
`s.discard( x ) ` 
>>>thisset = set(("Google", "Runoob", "Taobao"))  
>
>>> thisset.discard("Facebook")  # 不存在不会发生错误  
>
>>> print(thisset)
{'Taobao', 'Google', 'Runoob'}   
  
我们也可以设置随机删除集合中的一个元素，语法格式如下：  
    s.pop()    

    thisset = set(("Google", "Runoob", "Taobao", "Facebook"))  
    
    x = thisset.pop()  
    
     
    print(x)    
输出结果：    

    $ python3 test.py   
    
    Runoob
      
3 ##判断语句    
根据Python的缩进规则，如果if语句判断是True，就把缩进的两行print语句执行了，否则，什么也不做。
也可以给if添加一个else语句，意思是，如果if判断是False，不要执行if的内容，去把else执行了
可用elif做更详细的判断，elif是else if的缩写
if语句执行有个特点，它是从上往下判断，如果在某个判断上是True，把该判断对应的语句执行后，就忽略掉剩下的elif和else

 4、三目表达式
为真时的结果 if 判定条件 else 为假时的结果


5、循环语句
5.1 while循环
5.1.1 常见while循环


5.1.2 while的else语句
当while循环正常执行完毕，接着会执行else语句


5.1.3 while的break
若存在break，会强制提前终止循环，也不会执行后面的else语句


5.2 for循环
5.2.1 常见for循环
for循环通常用来遍历可迭代的对象，如一个列表或一个字典


5.2.2 for循环的嵌套语句


5.3 循环中的break语句
break只能用于循环体内，作用是达到break条件则直接结束并退出当前循环（只能退出一层循环），剩下的未循环的工作全部被忽略与取消


5.4 循环中的continue语句
continue语句只能用于循环体内，作用是达到continue条件则跳过当前轮次循环的剩余部分代码，直接开始下一轮循环
