---
title: String Handling
description: strings
weight: 12
lastmod: 2022-11-20T10:23:30-09:00
draft: false
vimeo: 773632607
emoji: 🎭
video_length: 2:56
quiz: true
free: true
---

<quiz-modal options="96:97:98:99" answer="98" prize="5">
  <h6>What is 'b' ASCII Code?</h6>
</quiz-modal>

#### 1) What is ASCII Code?

ASCII stands for American Standard code for Information Interchange. ASCII character range is 0 to 255. 
We can’t add more characters to the ASCII Character set. ASCII character set supports only English. That 
13
is the reason, if we see C language we can write c language only in English we can’t write in other 
languages because it uses ASCII code.

#### 2) What is Unicode ?

Unicode is a character set developed by Unicode Consortium. To support all languages in the world Java 
supports Unicode values. Unicode characters were represented by 16 bits and its character range is 0-
65,535.
Java uses ASCII code for all input elements except for Strings,identifiers, and comments. If we want to 
use telugu we can use telugu characters for identifiers.We can enter comments in telugu.

#### 3) Difference between Character Constant and String Constant in java ?

Character constant is enclosed in single quotes. String constants are enclosed in double quotes. Character 
constants are single digit or character. String Constants are collection of characters.

Ex :’2’, ‘A’
Ex : “Hello World”

#### 4) What are constants and how to create constants in java?

Constants are fixed values whose values cannot be changed during the execution of program. We create 
constants in java using final keyword.

Ex : final int number =10;
final String str=”java-interview –questions”