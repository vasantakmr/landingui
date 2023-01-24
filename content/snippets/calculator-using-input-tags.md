---
title: Calculator using input 
lastmod: 2023-01-24T12:03:21-07:00
publishdate: 2023-01s-24T12:03:21-07:00
author: Vasanta Kumar
draft: false
description: Build a calculator using input tags
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
    <table>  
        <tr>
            <td>
                <label> Enter First value</label> 
                <input type="text" id="f_value" name="">
            </td>
            <td>
                <label> Enter Second value</label>
                  <input type="text" id="s_value" name="">
            </td>
            <td>
                <label>Result</label> <input type="text" id="result" name="">
            </td>
        </tr>
    </table>

    <input type="button" id="add" value="Addition" onclick="calculate(1);" name="">
    <input type="button" id="sub" value="Subtraction" onclick="calculate(2);" name="">
    <input type="button" id="mul" value="Multifunction" onclick="calculate(3);" name="">
    <input type="button" id="duvi" value="Division" onclick="calculate(4);" name="">


    <script type="text/javascript">

        function calculate(choice) {
            console.log(document.getElementById("f_value").value)
            var n1;
            n1 = Number(document.getElementById("f_value").value);
            var n2;
            n2 = Number(document.getElementById("s_value").value);
              var fresult; 
              switch (choice) {
                case 1: fresult = n1 + n2; break; 
                case 2: fresult = n1 - n2; break; 
                case 3: fresult = n1 * n2; break; 
                case 4: fresult = n1 / n2; break;
            } 
            document.getElementById("result").value = fresult; 
        }    
    </script>
</body>

</html>
```
