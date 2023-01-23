---
title: Operators
description: operators
weight: 3
lastmod: 2022-11-20T10:23:30-09:00
draft: false
youtube: zBZgdTb-dns
emoji: ⚡
video_length: 2:30
quiz: true
free: true
---

<quiz-modal options="Logical AND:Logical OR:Bitwise OR:Bitwise AND" answer="Logical AND" prize="1">
  <h6>What is && operator?</h6>
</quiz-modal>

#### 1) Difference between ‘>>’ and ‘>>>’ operators in java?

'>>' is a right shift operator shifts all of the bits in a value to the right to a specified number of times.

int a =15;
a= a >> 3;

The above line of code moves 15 three characters right.

`> > >` is an unsigned shift operator used to shift right. The places which were vacated by shift are filled 
with zeroes.


#### 2) What is the difference between the "==" and "===" operators in Java?

The "==" operator compares the values of two variables to see if they are equal, while the "===" operator compares the references of two variables to see if they point to the same object in memory.

#### 3) What is the difference between the "&" and "&&" operators in Java?

The "&" operator is a bitwise operator, while the "&&" operator is a logical operator. The "&" operator compares each bit of the first operand to the corresponding bit of the second operand, while the "&&" operator only evaluates the second operand if the first operand is true.

#### 4) What is the difference between the "|" and "||" operators in Java?

The "|" operator is a bitwise operator, while the "||" operator is a logical operator. The "|" operator compares each bit of the first operand to the corresponding bit of the second operand, while the "||" operator only evaluates the second operand if the first operand is false.

#### 5) What is the difference between the "^" operator and the "!" operator in Java?

The "^" operator is a bitwise operator that compares each bit of the first operand to the corresponding bit of the second operand, while the "!" operator is a logical operator that negates the value of a boolean expression.

#### 6) How does the "instanceof" operator work in Java?

The "instanceof" operator checks if an object is an instance of a certain class or one of its subclasses. It returns true if the object is an instance of the specified class, and false otherwise.

#### 7) What is the difference between the "<<" and ">>" operators in Java?

The "<<" operator is a bit shift operator that shifts the bits of the first operand to the left by the number of positions specified by the second operand. The ">>" operator is a bit shift operator that shifts the bits of the first operand to the right by the number of positions specified by the second operand.

#### 8) How does the "+=" operator work in Java?

The "+=" operator is a shorthand operator that is used to add the value of the right operand to the value of the left operand, and then assigns the result to the left operand. For example, the statement "x += y" is equivalent to "x = x + y".

#### 9) How does the "-=" operator work in Java?

The "-=" operator is a shorthand operator that is used to subtract the value of the right operand from the value of the left operand, and then assigns the result to the left operand. For example, the statement "x -= y" is equivalent to "x = x - y".

#### 10) How does the "*=" operator work in Java?

The "*=" operator is a shorthand operator that is used to multiply the value of the left operand by the value of the right operand, and then assigns the result to the left operand. For example, the statement "x *= y" is equivalent to "x = x * y".

#### 11) How does the "/=" operator work in Java?

The "/=" operator is a shorthand operator that is used to divide the value of the left operand by the value of the right operand, and then assigns the result to the left operand. For example,the statement "x /= y" is equivalent to "x = x / y".

