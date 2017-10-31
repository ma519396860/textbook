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
* 为了得到一个字符串的第N个字符，你可以获取该字符串的长度并减N来作为最后一个字符的索引。
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
* Math.random()用来生成一个在0(包括0)到1(不包括1)之间的随机小数，因此Math.random()可能返回0但绝不会返回1。
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
* 在JavaScript中, 数字选择器类似于: /\d/g。
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
* 浏览器会运行script里所有的Javascript，包括jQuery。
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
* 学习方法的应用。
appendTo() 移动HTML元素
clone() 复制元素
* 操作父级元素与子级元素
每个HTML元素都有一个parent元素，并从中继承属性。
如：< body>
< div class="container-fluid">
< h3 class="text-primary text-center">jQuery Playground< /h3>
< /div>
h3的父级元素是div，而div的父级元素是body；
每个HTML元素都是body的子元素，h3元素是< div class="container-fluid">的子元素。
* parent()方法 可以设定一个HTML元素的父级元素的css样式；
("#left-well").parent().css("background-color", "blue")
* children()方法 可以设定一个HTML元素的子级元素的css样式；
("#left-well").children().css("color", "blue")
##初级脚本算法
1.  翻转字符串
* function reverseString(str) {
 str = str.split('');  //字符串转化为数组
  str = str.reverse();   //翻转数组顺序
  str = str.join('');  //数组转为字符串

  return str;
}
reverseString("hello");
2.  阶乘算法
* function factorialize(num) {
  var s=1;
  for (var i=1;i<=num;i++) {
      s=s*i;  
  }
    return s;
}
factorialize(5);
3.  回文算法挑战
* function palindrome(str) {
// Good luck!
  var  str1 = str.toLowerCase();  //小写  
  var reg = /[\W\_]/g;  //  /\W/ 为删除所有非字母数字字符，匹配一个非单字字符;/\_/g 匹配下环线。那么正则式 /[\W\_]/g 能满足测试用例的需求。  
  var str2 = str1.replace(reg, "");//去掉非字母和非数字等  
  var str3 = str2.split("");  //字符串分隔成数组  
  var str4 = str3.reverse();  //反转数组中的元素  
  var str5 = str4.join("");    //反转后的数组转化为字符串  
 
  return str2 === str5; //如果测试用例是回文，返回 true；反之，返回 false。
}
palindrome("eye");
4.  寻找最长的单词算法挑战
* function findLongestWord(str) {
var arr = str.split(" ");  
var max=0;  //设置一个中间值max
for (var i = 0; i <arr.length; i++) { //遍历数组
    if(arr[i].length>max)
    {
        max=arr[i].length;   //遍历且每次比较把长度最长的赋给max
    }
}
return max;
}
findLongestWord("The quick brown fox jumped over the lazy dog");
5.  设置首字母大写算法挑战
* function titleCase(str) {
             var arr = str.toLowerCase().split(" ");//以小写的形式将字符串转化为数组
             var newArr = [];
             for (var i = 0; i < arr.length; i++)  {//遍历数组
                 newArr[i] = arr[i].split("");将第i个索引位置上的字符转化为数组；
                 newArr[i][0] = newArr[i][0].toUpperCase();//将第i个一维数组的第1个字符转化为大写；
                newArr[i] = newArr[i].join("");//将第i个一维数组转化为字符串；
             }
             arr = newArr.join(" ");//将数组转化为字符串
             return arr;
         }
titleCase("I'm a little teapot");
6.  寻找数组中的最大值
* function largestOfFour(arr) {
var results = []; // 创建一个results变量来存储
// 创建一个外层循环，遍历外层数组
for (var n = 0; n < arr.length; n++) {
var max = 0; // 创建第二个变量，存储最大的数
// 创建另一个循环，遍历子数组
for (var s = 0; s < arr[n].length; s++) {
//检查子数组的元素是否大于当前存储的最大值
if (arr[n][s] > max) {
// 如果为真，将这个值赋予给变量max
max = arr[n][s];
}
}
// 内部循环后，将每个子数组中的值保存到数组results中
results[n] = max;
}
// 返回数组
return results;
}
largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
7.  确认末尾字符
*   function confirmEnding(str, target) {
var flag=true;
for(i=str.length-1,j=target.length-1; i>=0, j>=0;i--, j--)//从俩个数组的末尾开始比较
{
    if(str[i]!=target[j]){  //如果不相等 把false赋给flag 并退出循环；
        flag=false;
        break;
    }
}
return flag;
}
confirmEnding("Bastian", "n");
8.  重复操作算法
* function repeat(str, num)
   {
    var s="";
  for(var i=0;i<num;i++)   //根据num值控制循环的次数；

    { if(num<0)         //判断num是否为负数

  {
    return "";   //返回空字符串
  }
    
   s=s+str;         //拼接
     
  }
   return s;
 }
repeat("*", -4);
9.  字符串截取算法
* function truncate(str, num) {
            var result = '';   //定义一个空字符串
            var strArr = str.split('');  //将字符串转化为数组
            if(num<=3){      循环条件
                result = str.slice(0,num) +'...'; //num参数小于3，添加的三个点号不会计入字符串的长度。截取数组索引0-num位置的字符+字符串...赋值给result；
            }else if(str.length>num){                            //num参数大于3且字符串长度大于num参数，3个点计入，所以截止到num-3；
                result = str.slice(0,num-3) + '...';
            }else{                  //num >字符串的本身长度，全部输出。
                result = str;
            }
            return result;
}
truncate("A-tisket a-tasket A green and yellow basket", 3);
10. 数组分割算法
* function chunk(arr, size) {
var newArr = [];
            var index = 0,
                end = size;
            var count = arr.length / size;  //js整除也会显示小数；5/2=2.5//判断分为几个一维数组
            for (var i=0; i < count; index += size) {    //遍历数组
                newArr[i] = arr.slice(index, end);      //截取数组index-end
                end = end + end;              //end迭代
                i++;
            }
            return newArr;
}

chunk(["a", "b", "c", "d","e"], 2);
11. 数组截断算法
* function slasher(arr, howMany) {
// it doesn't always pay to be first
var str=[];
    str=arr.slice(howMany,arr.length) //截取
return str;
12. 数组查询算法
* function mutation(arr) {
 var c=0;//计算第二个字符串有几个字符和第一个字符串里的字符相等；
 var tag=true;    //返回值；
arr= arr.join(" ");  //将数组转化成字符串 用空格连接
arr=arr.toLowerCase().split(" "); //因为判断包含无关大小写，所以将转换后的字符串以小写形式的数组输出；
arr[0]=arr[0].split("");//将一维数组分割成二维数组；
arr[1]=arr[1].split("");//将一维数组分割成二维数组；
for(var i=0;i<arr[1].length;i++)    //控制第二个字符串总的循环次数；
{
    for(var j=0;j<arr[0].length;j++) //控制第二个字符串每一个字符同第一个字符串每一个字符比较的字数；
    {
     if(arr[1][i]==arr[0][j])
     {
         c++;                //俩个字符串字母是否相等，相等加一；中间值（中转站）；
         j=arr[0].length; //第二个字符串中字母找到第一个字符串里对应的字符，跳出本次循环；
     }
    }
}
if(c!=arr[1].length)  //判断第一个字符串是否包含第二个字符串
{
    tag=false;
}
return tag;
}
mutation(["hello", "hey"]);
13. 删除数组特定值（需加深理解）
* function bouncer(arr) {
var index = 0; // Don't show a false ID to this bouncer.
for (; index < arr.length; index++)
{ if (!arr[index])
{ 
    arr.splice(index, 1); 
    index--;//保证删除数组元素后，索引不跳过下一个 
}
}
return arr;   
}
bouncer([7, "ate", "", false, 9]);
14. 去除数组中任意多个值（需加深理解）
* function destroyer(arr,del1,del2,del3) {
 var newDel = [del1, del2, del3];    
            for (var index=0; index < newDel.length; index++) {
                var i = 0;
                for (; i < arr.length; i++) {
                    if (arr[i] == newDel[index]) {
                        arr.splice(i, 1);
                        i--;
                    }
                }
            }
            return arr;
}
destroyer([1, 2, 3, 1, 2, 3], 2, 3);
15. 数组排序并插入值算法（需加深理解）
* function where(arr, num) {
arr.push(num);
            for (var i=0; i < arr.length - 1; i++) {
                for (var j=i+1; j < arr.length; j++) {
                    if (arr[i] > arr[j]) {
                        var temp = arr[i];
                        arr[i] = arr[j];
                        arr[j] = temp;
                    }
                }
            }
            for (var index=0; index < arr.length; index++) {
                if (arr[index] == num) {
                    return index;
                }
            }
}
where([40, 60], 50);
16. 位移密码算法（需加深理解）
* function rot13(str) { /
        var result = [];
        for(var i=0;i<str.length;i++){
          if(str.charCodeAt(i) >= 65 && str.charCodeAt(i) <= 90)//使用charCodeAt()方法可以取得每个字符的Unicode值{
            var code = str.charCodeAt(i) + 13;
            if(code>90){
              code = str.charCodeAt(i) + 13 - 26;
            } 
            result.push(String.fromCharCode(code));
          }else{
            result.push(str[i]);
          }
        }
        return result.join("");
      }
rot13("SERR PBQR PNZC");
## 其他
1.  linux系统 ubuntub16.04版本的安装；
2.  配置并更新源；
3.  建立自己的github账号并使用，建立自己的库；
3.  vscode的安装与配置；连接自己的github账号，使vscode与gihub同步；
4.  建立自己的gitbook与github同步；
5.  在vscode中安装markdown插件，编辑自己的学习笔记；
6.  坚持英语流利说每日打卡；坚持每天进行代码训练营练习；