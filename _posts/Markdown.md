---
layout:     post
title:      Markdown Cheat Sheet
subtitle:   Syntax of Markdown Edition
date:       2021-01-03
author:     Jimeng
header-img: img/southeast_view.jpg
catalog: true
tags:
    - Markdown
---

[TOC]

# Title
    # Heading 1
    ## Heading 2
    ### Heading 3
    
# Heading 1
## Heading 2
### Heading 3


# Text
    Bold: **Bold text**
    Italic: *Italic text*
    Delete line: ~~Delete line~~
    World Highlight: This is a ==highlighted== word.

**Bold text**

*Italic text*

~~Delete line~~

'Highlighted text'


# Link
    [word](concrete link)  --> e.g.: [google](https://www.google.com/)
    ![](picture link)      --> e.g.: ![](images/demo.jpg){height=30%}
    ![](picture link)      --> e.g.: ![](images/demo.jpg){height=30%} \ ![](images/demo.jpg){height=10%}
    [![pic_name.png](online link of picture)](blog link where you want to post)
    [![wUUa9K.png](https://s1.ax1x.com/2020/09/12/wUUa9K.png)](https://jimengshi.github.io/2020/01/01/Introduction-to-Machine-Learning/)
    <div align="center">
    <img src="https://github.com/JimengShi/JimengShi.github.io/blob/master/img/Classification.png" alt="Classification" width=10%>
    </div>


# Code
    # Codes in multiple lines
    ```Python
    Codes
    ```
    
```Python
def addition(a, b):
    print("The sum is: ", a+b)
```    

    # Codes in a single line
    `Codes`
    
hahaha `print("Hello, world!")` hahaha


# Break Line
    # must be 3 or more
    *** or ---
    
--------------------    
    
# Table
    Column1 | Column2 | Column3
    :--------|:------:|-----
    e | d | d
    e | d | d
Column1 | Column2 | Column3
:--------|:------:|-----
e | d | d
e | d | d


# Check
    - [x] checked words
    - [ ] not checked words
    
- [x] checked words
- [ ] not checked words


