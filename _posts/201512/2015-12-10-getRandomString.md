---
layout: post
title: 获取指定位数的随机字符串
description: 前台js
categories:
-  WorkCode/page
tags:
- randomString
---

##工作中积累的常用代码##
###前台js###
###获取指定位数的随机字符串
如以下代码：  

	function getRnd(v) {  
		var s = ["0", "1", "2", "3", "4", "5", "6", "7", "8", "9", "A", "B", "C", "D", "E", "F", "G", "H", "I", "J", "K", "L", "M", "N", "O", "P", "Q", "R", "S", "T", "U", "V", "W", "X", "Y", "Z", "a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m", "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"];  
		var r = "";  
		for (var i = 0; i < v; i++) {  
		   r += s[parseInt(61 * Math.random())];  
		}  
		return r;  
	}
从指定字符集中获取指定位数的随机字符串