# My Curriculum Vitae
 Curriculum Vitae

> # Sasha Zaloga
> ## Age: 19

---
> ### Contacts 
* [VK](https://vk.com/zaloga1998)
* [GitHub](https://github.com/agarin6)
---
> ## Something About Myself:
I am reliable, hard working and an enthusiastic individual with a great passion for the software testing and developing industry. At this moment I live in Republic Of Belarus, the city of Mahilyow. I am a second-year student of the Belarusian-Russian University, study at Engineering and Economics Faculty, majoring in Software Engineering. I have excellent communication skills, enabling me to effectively communicate with a wide range of people with different temperaments of character.
---
> ### My Skills:
1. C#
2. T-SQL (Microsoft SQL Server, Microsoft Access)
3. Football skills  
4. Painting skills
---
> ### Language Skills:
1. English Level: A2 (According to EPAM English Test), B1 (According to A1QA English Speaking and Grammar Test)
2. Russian Level: C2 (Native Speaker)
3. Belarussian Level: C2 (Native Speaker)
---
> ### Solved CodeWars katas (Code examples)
* Write a function that accepts an integer n and a string s as parameters, and returns a string of s repeated exactly n times.
```
function repeatStr (n, s) {
 return s.repeat(n);
}
```
* Your job here is to write a function (keepOrder in JS/CoffeeScript, keep_order in Ruby/Crystal/Python, keeporder in Julia), which takes a sorted array ary and a value val, and returns the lowest index where you could insert val to maintain the sorted-ness of the array. The input array will always be sorted in ascending order. It may contain duplicates.
```
function keepOrder(ary, val) {
  let index = 0;
  while (index < ary.length && ary[index] < val) {
    index++;
  }
  return index;
}
```
* Some numbers have funny properties. For example: 89 --> 8¹ + 9² = 89 * 1 695 --> 6² + 9³ + 5⁴= 1390 = 695 * 2 46288 --> 4³ + 6⁴+ 2⁵ + 8⁶ + 8⁷ = 2360688 = 46288 * 51 Given a positive integer n written as abcd... (a, b, c, d... being digits) and a positive integer p we want to find a positive integer k, if it exists, such that the sum of the digits of n taken to the successive powers of p is equal to k * n. In other words: Is there an integer k such as : (a ^ p + b ^ (p+1) + c ^(p+2) + d ^ (p+3) + ...) = n * k If it is the case we will return k, if not return -1. Note: n and p will always be given as strictly positive integers.
```
function digPow(n, p){
  let digits = n.toString().split('');
  let sum = 0;
  for (let i = 0; i < digits.length; i++) {
    sum += Math.pow(parseInt(digits[i]), p + i);
  }
  let k = sum / n;
  return Number.isInteger(k) ? k : -1;
}
```