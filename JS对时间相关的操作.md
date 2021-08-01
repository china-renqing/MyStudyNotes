# JS对时间相关的操作

#### 基本操作

* **获取本地当前时间**

  * `let nowTime=new Date();`

* **将获取的时间转换为时间戳**

  * 转换为时间戳后可以进行后续的操作
    * 以下两种方法都可以获得时间戳，方法二获得的时间戳更加精确
    * 方法一：`let timestamp=Date.parse(nowTime);`
    * 方法二：`let timestamp=nowTime.valueOf();`

* **获取时间戳下的年、月、日等方法**

  * 没有将时间戳用Date包裹的话，是不能取到对应的方法的

  * 一般我们会接收到一个时间戳，我们会对时间戳进行如下处理来格式化日期

    * ```js
      function formateDate(timestamp){
          function formatDate(timestamp){
              //注意：下面的代码时必须的，不然后面的方法，时不能获取到的
              let date=new Date(timestamp)
              let year=date.getFullYear();
              let month=date.getMonth()+1;
              let days=date.getDate();
              let hours=date.getHours();
              let minutes=date.getMinutes();
              let seconds=date.getSeconds();
              let week=date.getDay();
              return `${year}年${month}月${days}日${hours}时${minutes}分${seconds}秒;星期${week}`
      	}
      }
      ```
  
* **其它方法的**

  * 因为对其它方法的不熟悉所以去别的地方逛了以下，找到一位大神写的，写的还很全，就把一部分粘贴了过来[点击此处直接前往原文链接](：https://blog.csdn.net/qq_26747571/article/details/53289120)

  * ```js
    var milliSeconds = now.getMilliseconds();//获取当前毫秒数(0-999)
    var now_date = now.toLocaleDateString();//获取当前日期: 2016/11/22
    var now_time = now.toLocaleTimeString();//获取当前时间: 下午5:35:55
    var date_time = now.toLocaleString( );//获取日期与时间: 2016/11/22 下午5:35:55
    var d = now.toDateString();//Wed Nov 23 2016
    var t = now.toTimeString();//15:11:30 GMT+0800 (中国标准时间)
    var d_t = now.toString();//Wed Nov 23 2016 15:11:30 GMT+0800 (中国标准时间)
    ```