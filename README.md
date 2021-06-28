# 什么是正则表达式
* 一种通用字符串匹配方式

# 如何创建正则对象
* 字面量形式 
```var reg = /3/;```
* 函数创建形式
```var reg = new RegExp('3');```

# 匹配模式 -- 也就是修饰符
## 修饰符
* i 忽视大小写
* g 全局查找
## 用法
```var reg = /3/i;```
```var reg = new RegExp('3', 'g')```

# 正则对象的方法
* test()
* exec()

# String 对象的方法
* match()
* search()
* replace()
* split()

# 几个重要概念
## 子表达式 
在正则表达式中，通过一对圆括号括起来的内容，我们称之为子表达式
## 捕获 
在正则表达式中，子表达式匹配到相应的内容时，系统会自动捕获这个行为，然后将子表达式匹配到的内容放入系统的缓存区中，我们把这个过程称之为捕获
## 反向引用 
在正则表达式中，我们可以使用 \n （n > 0，n 为整数，代表系统中的缓存区编号）来获取缓存区的内容，我们把这个过程称为反向引用

# 编写正则表达式
## 正则表达式组成 
正则表达式是由普通字符（例如字符 a 到 z）以及特殊字符（称为元字符）组成的文字模式，正则表达式作为一个模板，将某个字符模式与所搜索的字符串进行匹配
## 重要属性
1. 匹配区间
2. 限定符
3. 定位符
4. 转义字符
5. 或者的用法
6. 预查的用法
