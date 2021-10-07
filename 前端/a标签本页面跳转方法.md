# a标签本页面跳转方法

#### 使用Id和a标签搭配跳转

```html
<div id="pinkDiv" style="widht:100px;height:100px;background-color:pink">粉色盒子</div>
<div style="height:1000px">我是占位符</div>
<a href="#pinkDiv">跳转到粉色盒子</a>
```



#### 使用js的事件进行跳转

* ```html
  <button onclick="document.getElementById("bb").scrollIntoView">
      跳转
  </button>
  ```

#### Jquery方法

* 和js的事件跳转类似，获取对应的节点，然后调整滚动条，到指定节点位置即可。

