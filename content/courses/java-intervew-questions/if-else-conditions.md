---
title: If/else conditions 
description: If/else conditions concepts
weight: 4
lastmod: 2022-11-20T10:23:30-09:00
draft: false
youtube: TNhaISOUy6Q
emoji: ⚛
video_length: 2:30
free: true
quiz: true
---

<quiz-modal options="1:2:5:any" answer="any" prize="2">
  <h6>How many number nested if conditions can we have?</h6>
</quiz-modal>

#### 1) What is the basic syntax of an if-else statement in Java?
The basic syntax of an if-else statement in Java is as follows:

```java
if (condition) {
    // code to be executed if condition is true
} else {
    // code to be executed if condition is false
}
```

#### 2) How do you check for equality between two variables in a condition in Java?
To check for equality between two variables in a condition in Java, you can use the == operator. Example: if (x == y)

#### 3) How do you check for inequality between two variables in a condition in Java?
To check for inequality between two variables in a condition in Java, you can use the != operator. Example: if (x != y)

#### 4) How do you check if a variable is greater than or less than another variable in a condition in Java?
To check if a variable is greater than or less than another variable in a condition in Java, you can use the > or < operator respectively. Example: if (x > y) or if (x < y)

#### 5) How do you check if a variable is greater than or equal to, or less than or equal to another variable in a condition in Java?
To check if a variable is greater than or equal to, or less than or equal to another variable in a condition in Java, you can use the >= or <= operator respectively. Example: if (x >= y) or if (x <= y)

#### 6) How can you check if a variable is equal to multiple values in an if-else statement in Java?
You can use multiple if-else statements or you can use logical operator OR(||) between different conditions. Example: if (x == 1 || x == 2 || x == 3)

#### 7) How can you check if a variable is not equal to multiple values in an if-else statement in Java?
you can use logical operator AND (&&) between different conditions with negation. Example: if (!(x == 1 || x == 2 || x == 3))

#### 8) How do you use an if-else statement inside another if-else statement in Java?
You can use an if-else statement inside another if-else statement by placing the inner if-else statement within the block of the outer if-else statement.

#### 9) How do you use the ternary operator in an if-else statement in Java?
The ternary operator in Java is a shorthand way of writing an if-else statement. The syntax is: (condition) ? expression1 : expression2. If the condition is true, the ternary operator returns expression1, otherwise it returns expression2.

#### 10) How do you use a switch statement in place of an if-else statement in Java?
A switch statement in Java can be used in place of an if-else statement when you need to check a variable against multiple cases. The basic syntax is:

```java
switch (variable) {
    case value1:
        // code to be executed if variable is value1
        break;
    case value2:
        // code to be executed if variable is value2
        break;
    default:
        // code to be executed if variable is none of the above
}
```

#### 11) How do you use a nested if condition?

A nested if statement in Java is an if statement that is placed within the block of another if statement. The syntax is:
```java
if (condition1) {
    // code to be executed if condition1 is true
    if (condition2) {
        // code to be executed if condition2 is true
    }
}
```

#### 12) How do you use the logical operators AND (&&) and OR (||) in an if-else statement in Java?
The logical AND operator (&&) is used to check if both conditions are true, and the logical OR operator (||) is used to check if at least one condition is true. Example: if (condition1 && condition2) or if (condition1 || condition2)

#### 13) How do you use the logical NOT operator (!) in an if-else statement in Java?
The logical NOT operator (!) is used to negate a condition, making it the opposite of its original state. Example: if (!condition)
#### 14) How do you check if a variable is equal to null in an if-else statement in Java?
To check if a variable is equal to null in an if-else statement in Java, you can use the == operator. Example: if (variable == null)
#### 15) How do you check if a variable is not equal to null in an if-else statement in Java?
To check if a variable is not equal to null in an if-else statement in Java, you can use the != operator. Example: if (variable != null)
#### 16) How do you use the break statement in a switch statement in Java?
The break statement is used inside a switch case block to exit the switch statement, and it is optional. If the break statement is not used, the code execution will continue to the next case statement.

#### 17) How do you use the continue statement in a loop in Java?
The continue statement is used inside a loop to skip the current iteration of the loop and continue with the next iteration. It can be used inside a for, while, or do-while loop.