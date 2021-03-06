###0-Pow(x,n)
  
***
####问题：
  
实现pow(x,n)方法。即x的n次方运算。
  
####解决思路
  
***
使用二分的方式，即:  

```
if(n%2 === 0) {
	pow(x,n) = pow(x,n/2)*pow(x,n/2);
}
else {
	pow(x,n) = pow(x,(n-1)/2)*pow(x,(n-1)/2)*x;
}
```
  
####引申  
  
*** 
[解决该问题的5种方法](https://leetcode.com/discuss/52800/5-different-choices-when-talk-with-interviewers)

###1-Sqrt(x)
  
***
####问题：
  
实现sqrt(x)方法。即x的平方根。
  
####解决思路
  
***
1）使用二分的方式。（js下会超时？）
2）基于位运算（这是此处的解决方式）。首先，使用位移运算，找到使得```2^k * 2^k```小于x的最大值2^k，然后基于该数字的二进制表示，从高位到低位依次对其+1，直到找到乘积最接近x的那个值。

###2-Is Bad Version
  
***
####问题：
  
给定数字n，假设从1-n的某个整数开始，它和它之后的整数都是bad version，找出第一个bad version。
  
####解决思路
  
***
二分法查找，知道找到某个数字和它相邻数字测试badversion的结果不一样，那么较大的那个数就是我们要找的对象。  
[BadVersion-LeetCode](https://leetcode.com/problems/first-bad-version/¡)