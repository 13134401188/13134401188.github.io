---
layout:     post
title:      "整理---前端算法基础(一)"
subtitle:   "Front-end based algorithm"
date:       2020-02-20
author:     "Mr.Xi"
header-img: "img/post-bg-universe.jpg"
catalog:    true
tags:
    - JS
    - 前端 算法 
---

## 前言

>在开发中数据结构和算法是必不可少的一环，目前整理基础算法，后续逐步深入。

##### 1.判断一个字符串是否为回文
 * 回文是指类似于“上海自来水来自海上”或者“madam”，从前往后和从后往前读，字符串的内容是一样的，称为回文。判断一个字符串是否是回文有很多种思路：
 1.利用Array.reverse()反转数组特性
 ```python
       isPalindRome = (str)=>{
             console.log(str.split('').reverse().join('') === str);
             return str.split('').reverse().join('') === str;
       }
   ```  
 2.循环遍历对比
 ```python
        function isPalindRome(str) {
            let newStr = '';
            for(let i = str.length - 1; i >= 0; i --){
                newStr = newStr + str[i];
        
            }
            return newStr === str;
        
        }
        
        console.log(isPalindRome('madam'));//ture
        console.log(isPalindRome('mada'));//false
  ```  
 
##### 2.数组去重
 * JavaScript 中，函数及变量的声明都将被提升到函数的最顶部。
   JavaScript 中，变量可以在使用后声明，也就是变量可以先使用再声明。
   以下两个实例将获得相同的结果：
 
  ```python
      x = 5; // 变量 x 设置为 5
      
      elem = document.getElementById("demo"); // 查找元素
      elem.innerHTML = x;                     // 在元素中显示 x
      
      var x; // 声明 x
  ```  
  
  ```python
      var x; // 声明 x
      x = 5; // 变量 x 设置为 5
    
      elem = document.getElementById("demo"); // 查找元素
      elem.innerHTML = x; 
  ```     
