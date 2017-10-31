#泥巴综合实习10月总结
##html5&CSS
1.  标签与注释的学习。
2.  有序与无序列表
3.  form表单
* 单选按钮、多选按钮、文本框、提交按钮；
* 一个文本输入框设置为必填项在 input 元素中加上 required 属性，使用： 
input type="text" required
* 使用 checked 属性，可以设置一个单选框和复选框默认被选中。
4.  在< style>< /style>中为元素标签可以设置各种样式。
如：< style>
h2{color:blue;}
< /style> 为h2标签设置了蓝色的字体颜色。
5.  可以将class类应用到HTML元素中，且在style声明中，类选择器以.开头。
*  如：< style>
.red-text 
{
color: red;
}
< /style>
< h2 class="red-text">< /h2>
* 可以将一个Class类应用到多个html元素中。
* 也可以将多个class类应用到同一个HTML元素中去，只需要在多个class之间用空格分开即可。例如：
< img class="class1 class2">
* border-radius（边框半径）的CSS属性可以使边框变成圆角。
如：border-radius: 10px;还可以使用百分比来指定 border-radius（边框半径）的值，如border-radius: 50%;
6.  超链接的使用
7.  应用样式覆盖优先级：Important>内联样式>ID>Class(由上到下读取，后面的Class样式会覆盖前面的，如class2会覆盖掉class1的声明)>body;
8.  还有其他方式来表示CSS中的颜色，其中一种方式称为 hexadecimal code（十六进制编码）。 
* 总共，用 0 到 F 可以表示 hexadecimal 中的每一位数字，共为我们提供 16 个可能的数值。
在 CSS 中，我们可以使用 6 个十六进制数字来表示颜色，每 2 个分别表示红 (R)、绿 (G) 和蓝(B) 成分。
* 例如，#000000 是黑色，同时也是可能的数值中最小的。#FFFFFF是白色数字 
0是十六进制代码中最低的数字，表示完全没有颜色。。数字 F 是十六进制代码中最高的数字，表示最大可能的亮度。hex code（十六进制代码） 遵循 red-green-blue（红-绿-蓝）。
* 十六进制RGB表达式可以进行缩写。如：红色的十六进制码 #FF0000 可以缩短为 #F00。
9.  在 CSS 中表示颜色的另一个方法是使用 RGB 值。
* 代表黑色的 RGB 值如下所示：rgb(0, 0, 0)代表白色的 RGB 值如下所示：rgb(255, 255, 255)
* 使用 RGB，是使用RGB指定每个颜色的亮度，数字介于0到255之间，而不是像使用十六进制代码那样使用六个十六进制数字。
##JavaScript
1.  数据类型：undefined（未定义）, null（空）, boolean（布尔型）, string（字符串）, symbol(符号), number（数字）, and object（对象），共7种。
* 创建变量以Var开头，以；号结尾。
* 变量的名字：数字、字母、$ 或者 _组成，但是不能包含空格或者以数字为首。
* JavaScript 中所有的变量都是大小写敏感的。这意味着你要区分大写字母和小写字母。MYVAR与MyVar和myvar 是截然不同的变量。
* 使用驼峰命名法来命名变量。
* 可以使用变量名[索引数字]，获取该索引位置上的字符；如：firstName[0] 来获得第一个位置上的字符。（索引从0开始，0代表第一个字符）
* .length可以获取变量的长度。
2.  JavaScript 中，字符串的值是不可变的，这意味着一旦字符串被创建就不能被改变。改变的唯一方法是重新给它赋一个值。
*为了得到一个字符串的第N个字符，你可以获取该字符串的长度并减N来作为最后一个字符的索引。
如：firstName[firstName.length - N] 来得到字符串的最后的一个字符。
3.  数组
* 通过数组，我们可以将多个数据存储于同一个变量中。
* 定义数组：例如：var myArray = ["home",24];多维数组：var myArray = [ ["cat",22],["dog",24]];
* 数组索引：一维数组：var array = [1,2,3];array[0];// 等于 1
           多维数组：var myArray = [[1,2],3];
myArray[0];//等于[1,2]
                                             myArray[0][1];//等于2
* 数组的数据是可变的，并且可以自由地改变。如：var ourArray = [3,2,1];ourArray[0] = 1; //ourArray等于 [1,2,1]
* push（）函数追加数组数据。
将数据追加到一个数组末尾的最简单的方法是通过 push() 函数。
var arr = [1,2,3];arr.push(4);// 现在arr的值为 [1,2,3,4]
*pop() 函数，弹出数组最后数据，并可以把弹出的数据赋值给一个变量。
var oneDown = [1, 4, 6].pop(); //[1, 4]
* shift（）函数，移除数组第一个元素。
* unshift（）函数，移入一个元素到数组的头部。
var myArray = [ ["John", 23], ["dog",3]];myArray.unshift(["paul",35]);
4.  JavaScript函数定义
* 在 JavaScript 中，我们可以把代码的重复部分抽取出来，放   到一个函数（functions）中。
  如：function myFunction()

  {
    console.log("Hi World");
}
myFunction();  //每次调用myFunction()函数，就会输出Hi World
* 函数参数的调用；//实参决定形参
* 函数全局变量定义：作用域 影响着变量的作用范围。在函数外定义的变量具有全局作用域。这意味着，具有全局作用域的变量可以在代码的任何地方被调用。没有使用var关键字定义的变量，会被自动创建在全局作用域中，变成全局变量。
* 局部变量定义：在函数内部定义的变量只在函数内部有用。
如：function myTest() {
var loc = "foo";
console.log(loc);
}
myTest(); // "foo"
console.log(loc); // "undefined"；
* 一个程序中有可能具有相同名称的 局部变量和全局变量。在这种情况下，局部变量将会优先于全局变量。
如：var someVar = "Hat";
function myFun() {
var someVar = "Head";
return someVar;
}  //函数会返回Head；
* 全等于比较运算符===；和不全等比较运算符!==；它会同时比较元素的值和数据类型
如：3 === 3 // true
    3 === '3' // false
* 各种运算符和赋值符的应用；
* if语句的应用；
* switch语句的应用；
5.  对象操作；
* 对象和数组很相似，数组是通过索引来访问和修改数据，对象是通过属性来访问和修改数据的。
如：var cat = {
"name": "Whiskers",
"legs": 4,
"tails": 1,
"enemies": ["Water", "Dogs"]
};
对象适合用来存储结构化数据，存储一个对象的各种属性值。
* （.）操作符读取对象属性，如：var nameValue = cat.name;
* 也可以用（[]）操作符读取对象属性，你想访问的属性的名称有一个空格，这时你只能使用中括号操作符([])。
如：var drinkValue = testObj["the drink"];
属性名称中如果有空格，必须把属性名称用单引号或双引号包裹起来。
* 中括号操作符的另一个使用方式是用变量来访问一个属性，当你需要遍历对象的属性列表或查表时，这种方式极为有用。
var someProp = "propName";
var myObj = {
propName: "Some Value"
}
myObj[someProp]; // "Some Value"
* （.）和（[]）操作符还可以更新或者增加或删除对象属性；
* .hasOwnProperty(属性名)可以检查对象是否有该属性；
6.  JSON操作，获取JSON属性值，JSON数组值；
* 使用JavaScript对象的格式来存储数据。JSON是灵活的，因为它允许数据结构是字符串，数字，布尔值，字符串，和 对象 的任意组合。
var ourMusic = [
{
"artist": "Daft Punk",  //字符串
"title": "Homework",
"release_year": 1997,  //数字
"formats": [           //数组
"CD", 
"Cassette", 
"LP" ],
"gold": true           //布尔值
}
];
7.  for循环的应用；
8.  while循环的应用；
9.  random()生成随机小数
*Math.random()用来生成一个在0(包括0)到1(不包括1)之间的随机小数，因此Math.random()可能返回0但绝不会返回1。
10. 正则表达式；
* 正则表达式被用来根据某种匹配模式来寻找strings中的某些单词。
想要找到字符串The dog chased the cat中单词 the，可以使用下面的正则表达式: /the/gi
/ 是这个正则表达式的头部
the 是我们想要匹配的模式
/ 是这个正则表达式的尾部
g 代表着 global(全局)，意味着返回所有的匹配而不仅仅是第一个。
i 代表着忽略大小写，意思是当我们寻找匹配的字符串的时候忽略掉字母的大小写。
* 使用正则表达式选取数值
特殊选择器中的一种就是数字选择器\d，意思是被用来获取一个字符串的数字。
在JavaScript中, 数字选择器类似于: /\d/g。
在选择器后面添加一个加号标记(+)，例如：/\d+/g，它允许这个正则表达式匹配一个或更多数字。
尾部的g是'global'的简写，意思是允许这个正则表达式 找到所有的匹配而不是仅仅找到第一个匹配。
如：var expression = /\d+/g;
* 使用正则表达式选取空白字符
可以使用正则表达式选择器 \s 来查找一个字符串中的空白。
空白正则表达式类似于：
/\s+/g
如：var expression = /\s+/g //匹配所有空白字符
* 使用正则表达式反转匹配
可以用正则表达式选择器的大写版本来反转任何匹配（相反意思）。
例如：\s 匹配任何空白字符，\S 匹配任何非空白字符。
var expression = /\S/g; //匹配所有非空白字符
##Bootstrap
* Bootstrap会自动获取使用者屏幕的大小,并根据屏幕的大小自动调整HTML元素的宽度和高度来适配屏幕,因此称之为--响应式布局。
* 使用Bootstrap也非常简单,你只需要把下面的链接添加到你需要使用Bootstrap来进行布局的应用的头部：
< link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap /3.3.1/css/bootstrap.min.css"/>
* 给图片添加img-responsive 的class属性,图片的宽度就能自动适配屏幕的宽度啦。
* 给标签添加text-center的class属性,标题文字就可以居中了。
* 添加好看的按钮
* 样式的响应式应用
##jQuery
* 开始学习使用jQuery之前，需要在HTML文件中添加一些代码。
首先，在页面顶部添加一行script元素，然后在下一行写上结束符。
浏览器会运行script里所有的Javascript，包括jQuery。
在你的script元素里，添加这段代码：
< script>
    $(document).ready(function() {
    });
< /script>
function里面的代码会在浏览器加载页面后立即运行。
* jQuery语句，所有jQuery方法都是以美元符号开头
如：$("button").addClass("animated bounce");
//让所有的button元素有弹回效果，先用（“button"）来选择要改变的HTML元素，然后再用.addclass（）方法,可以给元素添加class。
* 三种获取元素的方式：type选择器("button")、class选择器(".btn")、id选择器("#target1")。
* removeClass()方法删除元素的class.
如：$("#target2").removeClass("btn-default");
* 设置元素不可用
.prop()方法禁用按钮；
如：$("button").prop("disabled", true);
* 学习多种方法的应用。
appendTo() 移动HTML元素
clone() 复制元素




