# DOM相关的操作

该篇笔记主要记录的是js相关DOM操作的代码

* **获取DOM节点**

  * 获取单个节点

    ```js
    let container=document.querySelector('.container')//通过类名获取
    let container=document.querySelector('#container')//通过Id获取
    let container=document.querySelector('li')//通过标签名获取，只获取第一个（单个节点获取）
    ```

  * 获取多个节点

    ```js
     let allDiv=document.querySelectorAll('div')//获取所有div盒子
     let allText=document.querySelectorAll('.text')//获取素有类名为text的元素
     let allIds=document.querySelectorAll('.ids')//获取素有id名为ids的元素
    ```

* **JS创造和插入DOM节点**

  * 最简单的节点插入方法

    ```js
    let div = document.querySelector('div')//获取父亲节点（等会插入到这里）
    let span=document.createElement('span')//创建一个box的
    span.innerHTML="你好"	 //给span标签写写入内容
    div.appendChild(span)//将创建的span标签插入到div盒子中
    ```

    