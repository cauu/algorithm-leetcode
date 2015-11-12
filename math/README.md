###0-Add Digits

***  
给一个非负整数，将其各位数字相加，若其结果扔大于等于时，重复之前的操作，直到得到一个小于10的数。
如:  

```
num = 38;
3 + 8 = 11;
1 + 1 = 2;
```
由于2小于10，因此返回2。
  
###解决思路
  
***
很简单的一道题。使用除法和求余运算将一个整数各位数字相加即可。

###1-Excel Sheet Column Number

***  
输出Excel表格列数代表的数字。  
如:  

```
    A -> 1
    B -> 2
    C -> 3
    ...
    Z -> 26
    AA -> 27
    AB -> 28 
```
  
###解决思路
  
***
相当于将26进制表示的数转换为10进制。