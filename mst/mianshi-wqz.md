# 租租车笔试(答案仅供参考，如有错误请告知让我纠正)
#### 一、单选题
 ```
    1.A
    思路：  
    用挡板法,做排列组合的基本方法每天至少吃1粒,则吃掉6粒,还有6粒可以自由选择,每加1块挡板,就分为2天,问题可转化为：将12个相同的小球放入6个盒子中,每个盒子至少一个,有多少种方法,因为去掉6个小球后只有6个小球,所以只有5个空隙不能用此方法,所以可直接在11个空隙里插入5个挡板,无顺序,即为11C6=(11×10×9×8×7×6）/(6×5×4×3×2×1）

    2.C
    思路：
    想在同一网段，必需做到网络标识(关键)相同,网络=标识算法只要把IP和子网掩码的每位数AND就可以了。
        AND方法：0和1=0　0和0=0　1和1=1
        ①首先将10.21.5.127 和255.255.0.0 转换为二进制，然后AND每一位(注：下面二进制空格只为便于阅读想自己测试请使用括号内的值)
          IP：1010.1 0101.101.111 1111           
             （1010.10101.101.1111111）
          子网掩码: 1111 1111.1111 1111.0000 0000.0000 0000      
                  （11111111.11111111.00000000.00000000）
          AND结果：00001010.00010101.00000000.00000000
        ②然后将AND结果十进制得出：10.21.0.0, 这就是网络表示符(关键)
        ③最后得出只要符合网络标识符：10.21.*.* 则正确( *处随便填只能用0和1填，不一定全是0和1)
        tip：有兴趣了解更多的可以访问：http://blog.sina.com.cn/s/blog_618199e60100ka5b.html

    3.如果会的 请帮忙补全(C语言或C++)

    4.D (不解释自己查课件)

    5.D
    思路：
    两个参数，首先按二进制位进行换算,然后每一位数进行"或"比较，位数不足以0补充
      运算方法：0|0=0；   0|1=1；   1|0=1；    1|1=1；
      即 ：只要有一个为1，其值为1。
      271 ：100001111      135：10000111
      则271|135 === 1 0000 1111|1000 0111
      得出比较后的二进制：110001111 转换为十进制得出答案 399；

    6.D (不解释 自己打代码验证)

    7.A
    思路：
    队列先进先出，队列始终是从front一段删除，并且从rear一段插入，因为如果从rear一段删除会找不到其上一个节点

    8.如果会的 请帮忙补全

    9.A
    思路：创建型
      1. Factory Method（工厂方法）
      2. Abstract Factory（抽象工厂）
      3. Builder（建造者）
      4. Prototype（原型）
      5. Singleton（单例）
      tip：有兴趣了解更多的可以访问：http://www.cnblogs.com/svennee/p/5057128.html

    10.B(略)

```
#### 二、多项选择题
```
    11.ACDE
    参考资料：http://blog.csdn.net/qq_27093465/article/details/52269862
        或http://blog.csdn.net/u012104435/article/details/47951357

    12.ABCDE
    思路：
    计算机科学中常用的编程范式(主流的):
    1.面向对象编程
    2.面向过程编程
    3.泛型编程
    tip：有兴趣了解更多的可以访问：http://blog.csdn.net/blues1021/article/details/47681307

    13.ABCE

    14.BE
```