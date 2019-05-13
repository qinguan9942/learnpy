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

#string字符串
定义及基本操作  
**所有标准的序列操作（索引，切片，乘法，成员资格检查，长度，最小值和最大值）都适用于字符串，但是字符串是不可变的因此所有的元素赋值和切片赋值都是非法的 **
（+*读取方式）
相关方法
字符串格式化
