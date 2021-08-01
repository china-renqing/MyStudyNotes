# C#方面的基础知识（控制台篇）

#### C#定义全局变量

* **以下是写全局变量的案例，注意全局变量需要添加static**

  * ```c#
    public static string[] coffees = new string[] { "浓咖啡", "混合咖啡", "重烘焙咖啡" };
    public static int[] coffeePrice = new int[] { 25, 30, 20 };
    public static string[] others = new string[] { "摩卡", "奶泡", "牛奶" };
    public static int[] otherPrice = new int[] { 10, 8, 6 };
    ```

#### 数组

* **定义数组数组**

  * 不定长写法
    * 以下两种写法的效果相同，如果提供了初始值设定，可以省略new运算符
    * `int[] numbers =new int[]{1,2,3,4,5};`
    * `int[] numbers={1,2,3,4,5};`

  * 定长写法

    * `int[] numbers=new int[3]{1,2,3};`

  * 多维数组定义

    * 不定长多维数组
    * `int[,] numbers=new int[,]{{1,2,3},{1,2,3},{1,2,3}};`
    * 定长多维数组
    * `int[,] numbers=new int[3,3]{{1,2,3},{1,2,3},{1,2,3}};`

  * 初始化写法使用

    * ```c#
      //如果是先赋值后使用,该写法是生成长度为3的全0数组,必须给长度,不给报错
      int [] numbers=new int[3];
      //这种定义方法的赋值写法
      numbers[0]=1;
      ```

    * 

* **定义字符串数组**

  * 不定长写法
    * 以下两种写法的效果相同，如果提供了初始值设定，可以省略new运算符
    * `string[] str={"A","B","C"};`
    * `string[] str=new string[]{"A","B","C"};`
  * 定长写法
    * `string[] str=new string[3]{"A","B","C"};`

* **定义对象数组**

  * `Object[] obj = new Object[] { 1, 2, 3, 4, 5 };`



#### C#获取变量类型

* 获取变量类型例子如下：

  * ```C#
    //第一种显示方法
    System.Type t=123.GetType();
    Console.WriteLine(t);
    //第二种方法
    Console.WriteLine(123.GetType());
    ```

#### 尝试转换

* **在转换时很多时候都会因为转换不成功导致程序崩溃，为了解决这个尴尬的问题，可以使用TryParse。**
  * 例：尝试将字符串变量`str`尝试转换为数字变量`numbers`，`numbers`和`str`在调用前都需要已声明；
  * `int.TryParse(str,out numbers);`
    * 需要注意的是，它是拥有返回值的，它的返回值是一个布尔值类型的，成功为true，否则为false；`number`转换成功是对应数字，转换失败则为0；
  * 如果想更深刻了解TryParse，本人附上链接：[TryParse深度解析](https://blog.csdn.net/u010533180/article/details/52918126)

#### 程序暂停

* `Console.ReadLine()`;，当程序运行到这里时，程序自动停止。



该笔记仅当我在写咖啡店[装饰器模](https://www.runoob.com/design-pattern/decorator-pattern.html)式时，自己在敲代码不够熟练的部分，附上已经上传到了的GitHub的装饰模式代码：

[由控制台应用完成的简易咖啡店计算费用功能]([learn-MVC/装饰器/CofeeDecoratorDemo at master · china-renqing/learn-MVC (github.com)](https://github.com/china-renqing/learn-MVC/tree/master/装饰器/CofeeDecoratorDemo))