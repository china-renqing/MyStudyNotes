# Flex布局撑满全屏的方案

#### 方案一（撑满全屏加盒子居中）

* CSS部分

  * ```css
    *{
        margin: 0;
        padding: 0;
    }
    html,body{
        height: 100%;
    }
    .container{
        display: flex;
        height: 100%;
        background-color: pink;
        justify-content: center;
        align-items: center;
    }
    .content{
        display: flex;
        border: 1px solid black;
        width: 50%;
        height: 50%;
        border-radius: 3%;
        background-color: #00acec;
    }
    ```

  * 

* HTML部分

  * ```html
    <body>
        <div class="container">
            <div class="content"></div>
        </div>
    </body>
    ```

  * 