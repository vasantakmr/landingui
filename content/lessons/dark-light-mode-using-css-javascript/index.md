---
title: Dark/Light Mode using CSS and Javascript
lastmod: 2023-05-05T13:22:42-07:00
publishdate: 2023-05-05T13:22:42-07:00
author: Vasanta Kumar
draft: false
description: Simple implementation of dark/light theme switching functionality in a website.
tags: 
    - css
    - javascript
    - projects
    - web-development

# youtube: -atblwgc63E
# github: 
# disable_toc: true
# disable_qna: true

# courses
# step: 0

# versions:
#    rxdart: 0.20
---


{{< file "html" "index.html" >}}
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Dark Mode</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Light/Dark Mode Demo</h1>

    <button class="theme-toggler">Swith to Dark Mode</button>

    <script src="main.js"/>
</body>
</html>
```

{{< file "css" "style.css" >}}
```css
body {
    color: rgb(30, 32, 41);
    background-color: rgb(218, 218, 218);
    font-family: Arial, Helvetica, sans-serif;
}

.dark-mode {
    background-color: rgb(30, 32, 41);
    color: rgb(218, 218, 218);
}

button {
    color: rgb(215, 215, 215);
    background-color: rgb(40, 45, 61);
}

.dark-mode button {
    color: rgb(40, 45, 61);
    background-color: rgb(215, 215, 215);
}
```

{{< file "js" "main.js" >}}
```js
var toggleButton = document.getElementsByClassName("theme-toggler")[0];

toggleButton.addEventListener("click", toggleTheme);

function toggleTheme() {
    document.querySelector("body").classList.toggle("dark-mode");
    toggleButton.textContent = (toggleButton.textContent === "Switch to Light Mode")? "Switch to Dark Mode" : "Switch to Light Mode";
}
```

### Result

{{< figure src="img/dark-light-mode.gif" caption="Dark-Light Mode" >}}
