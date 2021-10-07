# JQuery的学习

#### 选择器

* :gt(index)

  * 匹配所有大于给定索引值的元素

* :lt(index)

  * 匹配所有小于给定索引值的元素

* :header

  * 匹配如h1,h2,h3的标题元素

* :animated

  * 匹配所有正在执行动画效果的元素
    * 思路：可以利用这个对不在执行动画效果的元素执行一个动画效果。

* :root

  * 文档根元素，永远是HTML

* :contains(text)

  * 匹配包含给定文字的元素

* :empty

  * 匹配所有不包含子元素或者文本的空元素

* :has

  * 匹配含有选择器所匹配的元素的元素
    * 例如：`$("div:has(p)")`意思就是找出所有包含p标签的div

* :parent

  * 匹配含有子元素或者文本的元素

* :hidden

  * 匹配所有含有不可见的元素，或者type为hidden的元素

* :visible

  * 查找所有可见的元素

* [attribute]

  * 匹配包含给定属性的元素

    > 例如：`$("div[id]")`

* [attribute=value]

  * 匹配所有包含给定的属性是某个特定值的元素

    > 例如：`$("input[name='hello']")`

* [attribute!=value]

  * 匹配所有包含给定的属性不是某个特定值的元素

* [attribute^=value]

  * 匹配给定的属性是以某些值开始的元素

* [attribute$=value]

  * 匹配给定的属性是以某些值结尾的元素

* [attribute*=value]

  * 匹配给定的属性是以包含某些值得元素

* `[selectore1][selectore2][selector3]`

  * 符合属性选择器，需要同时满足多个条件时使用

    > 例如：`$("input[id][name='man']")`

* :first-child      (:last-child)

  * 匹配所给选择器<span style="color:red">（:之前得选择器）</span>的第一个（最后一个）子元素
  * 类似的:first匹配第一个元素，但是:first-child选择器可以匹配多个：即为每个父级元素匹配第一个子元素。这相当于:nth-child(1)。（:last-child同理）

* 



#### 未理解

* :lang
* :focus
* :target