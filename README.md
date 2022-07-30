# <center>forge 中本聪实验报告</center>

>**课程名称     <u>创新创业实践课程</u>  **       
>
>**学生姓名   <u>李路岩</u>      学号  <u>202022180198</u>**     
>
>**学院   <u>网络空间安全</u>学院    专业  <u>信息安全</u>**   

[TOC]

## <center>实验思路</center>

>	**此实验采用了RSA签名的方式，伪造身份**

## **<center>关键代码</center>**

```python
    key_size = 272
    p = Generate_prime(key_size)
    print('p:',p)
    q = Generate_prime(key_size)
    print('q:', q)
    n, e, d = KeyGen(p, q)

    # 消息
    x = int(input("Message: "))
    # 签名
    s = Sign(x, d, n)
```



## <center>实验结果</center>

<a href="https://img.gejiba.com/image/EyjUIi"><img src="https://img.gejiba.com/images/470b9c5a52af39116de01b3de293fd90.png" alt="470b9c5a52af39116de01b3de293fd90.png" border="0"></a>
