```python
#转义字符案例
s = "let's go"
print(s)
```

    let's go
    


```python
s = 'let\'s go'
print(s)
```

    let's go
    

# 常见的转义字符
- \续行符
- \ 反斜杠
- \' 单引号
- \" 双引号
- \a 响铃
- \b 退格
- \000 空
- \n 换行
- \v 纵向制表符
- \t 横向制表符
- \r 回车
- \f 换页


```python
#单个反斜杠的用法
#python中，单个反斜杠表示此行未结束，出于美观，需要下一行继续
def myDemo(x,\
           y,\
           z):
    print("hahahaha")
myDemo(1,2,3)
```

    hahahaha
    

# 格式化
- 把字符串按照一定格式进行打印或填充
- 格式化分类：
    - 传统格式化
    - format
    
# 字符串的传统格式化方法
- 使用%进行格式化



```python
#%s进行简单的字符串替换
s = "I Love %s"
print(s%"王晓静")
```

    I Love 王晓静
    


```python
print("I love %s" % "李晓静")
```

    I love 李晓静
    


```python
s = "刘大拿今年 %d 岁了"
print(s % 19)
```

    刘大拿今年 19 岁了
    


```python
#如果格式化的信息多于1个，则用括号括起来就可以
s = "I am %fkg weight, %fm heigh"
print(s%(78,1.84))
```

    I am 78.000000kg weight, 1.840000m heigh
    


```python
#要规定小数点后面有几位 %.几f 就规定了小数点后面的位数
s = "I am %.2fkg weight, %.2fm heigh"
print(s%(78,1.84))
```

    I am 78.00kg weight, 1.84m heigh
    

# format 格式化
- 使用函数进行格式化，代替以前的百分号


```python
#方式1
s = "{} {}"
print(s.format("hello","world"))

#方式2
s = "{} {}".format("hello","world")
print(s)

#设置指定位置
s = "{0} {1}".format("hello","world")
print(s)
s = "{0} {0}".format("hello","world")
print(s)
s = "I love {0} and {0} loves me".format("王晓静")
print(s)
```

    hello world
    hello world
    hello world
    hello hello
    I love 王晓静 and 王晓静 loves me
    


```python
#通过字典设置参数，需要解包
s = "我们是{school_name},我们的网址是{url}，{teacher}最帅"
s_dict={"school_name":"北京图灵学院"，\
         "url":"www.",\
         "teacher"}
```
