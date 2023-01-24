---
title: Calculator using DIV 
lastmod: 2023-01-24T12:03:21-07:00
publishdate: 2023-01s-24T12:03:21-07:00
author: Vasanta Kumar
draft: false
description: Build a calculator using div
tags: 
    - html
    - css
    - javascript

code: 
type: lessons
---



{{< file "html" >}}
```html
<html>

<body>
    <div class="box outerbox">
        <div class="box bigBox"></div>
        <div class="box smallBox">1</div>
        <div class="box smallBox">2</div>
        <div class="box smallBox">3</div>
        <div class="box smallBox">4</div>
        <div class="box smallBox">5</div>
        <div class="box smallBox">6</div>
        <div class="box smallBox">7</div>
        <div class="box smallBox">8</div>
        <div class="box smallBox">9</div>
        <div class="box smallBox operation">+</div>
        <div class="box smallBox">0</div>
        <div class="box smallBox equal">=</div>
    </div>

    <script type="text/javascript">
        var num1 = 0;
        var num2 = 0;

        for (let index = 0; index < document.getElementsByClassName("smallBox").length; index++) {
            document.getElementsByClassName("smallBox")[index].addEventListener("click", m1);
        }

        function m1(e) {

            if(e.target.textContent == "+") {
                num1 = Number(document.getElementsByClassName("bigBox")[0].textContent);
                console.log("num1 is" ,num1)
                document.getElementsByClassName("bigBox")[0].textContent = "";
            } else if(e.target.textContent == "=") {
                num2 = Number(document.getElementsByClassName("bigBox")[0].textContent);
                console.log("num2 is" ,num2)
                
                document.getElementsByClassName("bigBox")[0].textContent = add();
            } else {
                document.getElementsByClassName("bigBox")[0].textContent += e.target.textContent;
            }
            
        }

        function add() {
            return num1 + num2;
        }
    </script>
</body>

</html>
```
