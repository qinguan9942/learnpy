#task2
##1列表
  序列是Python中最基本的数据结构。序列中的每个元素都分配一个数字 - 它的位置，或索引，第一个索引是0，第二个索引是1，依此类推。
列表和元组是python中常见的两个内置序列类型。  
序列都可以进行的操作包括索引，切片，加，乘，检查成员

**列表**是最常用的Python数据类型，它可以作为一个方括号内的逗号分隔值出现。
列表的数据项不需要具有相同的类型  

***创建***一个列表，只要把逗号分隔的不同的数据项使用方括号括起来即可
    list=['python','lemon',111,007]  

与字符串的索引标准语言，列表的索引从0开始。列的可以进行截取，组合等。  
append()方法可对列表的数据项进行更新或修改  
  

    list = []
    list.append('python')
    list.append(1)
    print list
    	['python',1]
 del()方法可删除列表中的元素  
        
    list=['python','day2',2,'day',9942]
	print list
	del list[2]
	print "after deleting value at index 2 :"
	print list  
输出结果

['python','day2',2,'day',9942]  
after deleting value at index 2 :  
['python','day2','day',9942]
    
  
  
  
拷贝  
    
      list1 =[1,2,3,4]      
      list2=[]  
      b=list1.copy(list1)  
	>>>b  
	[1,2,3,4]这里也可以使用类似a[:]切片进行复制

Python包含以下方法:  

方法
1 list.append(obj)在列表末尾添加新的对象  

2 list.count(obj)统计某个元素在列表中出现的次数  

3 list.extend(seq)在列表末尾一次性追加另一个序列中的多个值（用新列表扩展原来的列表）  

4 list.index(obj)从列表中找出某个值第一个匹配项的索引位置  

5 list.insert(index, obj)将对象插入列表  

6 list.pop([index=-1])移除列表中的一个元素（默认最后一个元素），并且返回该元素的值  

7 list.remove(obj)移除列表中某个值的第一个匹配项  

8 list.reverse()反向列表中元素   
 

9 list.sort(cmp=None, key=None, reverse=False)对原列表进行排  
序

#2元组
标志同列表一样 元组只是一个不可修改的序列  

基本操作     
 
创建 >>>(1,2,3)这便创建了一个元组，与列表不一样的是一个元素的元组形式为（1,）逗号不能省略  
元组的访问同列表一样  
元组的切片也是元组  

 
#3 String
　String 是定义一个字符串对象（内存中的字符串都是一个对象。）
　String 一旦被初始化就不能被改变（可以改变变量指向，但是不能改变对象内容）
　
定义方式： String s1 = “abc”; //在内存中存在一个对象。
String s2 = new String(“abc”)//在内存中存在两个对象。
　　　　　　　　 String s3 = “abc”;

二、字符串的常见方法
1、获取：字符串中包含的字符数（也就是字符串的长度）
int length(); (注意与数组中的length做区别，数组中为属性，字符串中为方法)

2、判断

2.1、判断字符串中是否包含指定字符串
boolean	contains(CharSequence s) ：CharSequence：为String实现的接口

3、转换
将字符数组转换成字符串
构造函数： String(char[] value)
String(char[] value, int offset, int count)： 将数组中从下标offset开始，一共count位字符转换成字符串。

4、替换
　String	replace(char oldChar, char newChar) ： 返回一个数组，它是用newChar 替换就数组中的oldchar等到的。（一个一个的替换）
String replace(CharSequence target, CharSequence replacement) ： 后替前，用新串替换原串中的子串。

注：原字符串没有改变，只是新出现了一个替换后的字符串（字符串一旦初始化，不能改变）	
如果要替换的字符没有，还是返回原串，不会生成新的字符串。

5、切割，分割

String[]	split(String regex) ： 指定其中某一个字符或字符串，以其下刀，切割字符串（其实应当依据正则表达式规则拆分）

6、子串：（获取一个字符串的一部分）

String	substring(int beginIndex) //从指定下标位置到结尾。
String	substring(int beginIndex, int endIndex) //从指定下标位置到结束下标位置前一个

7、转换、去除空格、比较

7.1：将字符串转换成大写或者小写。
String toUpperCase()
String toLowerCase()
7.2：将字符串两端多余的空额去除。
　　　　　　　　　　　String	trim()
7.3：将两个字符串进行自然顺序的比较。
　　　　　　　　　
int	compareTo(String anotherString)
int	compareToIgnoreCase(String str) ：不考虑大小写。


