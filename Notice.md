# 这是我在学习JavaScript中遇到的问题和相应的解决方案
***
## <font color=#008080>2017年10月19日</font>
###  在Alert中实现换行 例如：
<pre><script type="text/javascript">
  var mya,mya2;
  mya=5;
  mya2=15;
  alert("mya的值是:"+mya+"\n"+"mya2的值是:"+mya2);
</script></pre>
***
## 2017年10月20日
### ==(是否相等)是比较操作符 !=(是否不等)是比较操作符，输出true或false(不是1或者0)
***
## <font color=#008080>2017年10月26日</font>
### for循环中用;符号分隔条件不要用成逗号"," 例如:
<pre><script type="text/javascript">
var myarr=new Array();
for(var i=0;i<3;i++){
    myarr[i]=new Array();
    for(var j=0;j<6;j++);
    myarr[i][j]=i*j;
}
document.write("第三行第六个数组值为:"+myarr[2][5]);
</script></pre>
***
## 2017年10月29日
### JS输出加入换行符 如:
<pre><script type="text/javascript">
 //创建数组
 var arr=["*","##","***","&&","****","##*"];
 arr[7]="**";
 //显示数组长度
alert(arr.length);
document.write(arr[0]+"<br/>");
document.write(arr[7]+"<br/>");
document.write(arr[2]+"<br/>");
document.write(arr[4]+"<br/>");
</script></pre>
***
### switch else 如果没有break 将会从选择的case继续往下运行下去
<pre>var myweek =7;
switch(myweek)
{
 case 1:
 case 2:
 document.write("学习理念知识");
 break;
 case 3:
 case 4:
 document.write("到企业实践");
 break;
 case 5:
 document.write("总结经验");
 break;
 case 6:
 case 7:
 document.write("周六、日休息和娱乐");
 break;
 default:
 document.write("星期八?");
}
</script></pre>
***
## 2017年10月30日
### js事件文本发生改变 oninput()要比onchange()好用
***
### var声明的变量无法知道是字符串还是数字，使用parseInt()函数能转化为整数 如：
<pre><script type="text/javascript">
 function count(){
     var a=document.getElementById('txt1').value;
     var b=document.getElementById('txt2').value;
     var c=document.getElementById('select').value;
     var d;
     if (c=="+"){
         d=parseInt(a)+parseInt(b);
     }
     else if(c=="-"){
         d=parseInt(a)-parseInt(b);
     }
     else{
         d=parseInt(a)/parseInt(b);
     }
     document.getElementById('fruit').value=d;
 }
</script></pre>
***
## 2017年11月2日
### getTime()最后是毫秒所以在设置时间要精确到毫秒
<pre><script type="text/javascript">
 var mydate=new Date();
  document.write("当前时间："+mydate+"<br>");
  mydate.setTime( mydate.getTime()  + 2* 60 * 60 * 1000);
  document.write("推迟二小时时间：" + mydate);
</script></pre>
***
## 2017年11月3日
### Math.random()返回的是0-1之间的随机数，0-10之间的随机数要*10
***
## 2017年11月4日   EConf 前端开发者分享会
### 关键词： express RxJS 微组建开发 异步 面向对象 Ruby中国 rails社区
***
## 2017年11月5日
### 数组的排序 myArray.sort(sortMethod)方法
<pre><script type="text/javascript">
  function sortNum(a,b) {
  return a - b;   //升序，如降序，把“a - b”该成“b - a”
}
 var myarr = new Array("80","16","50","6","100","1");
  document.write(myarr + "<br>");
  document.write(myarr.sort(sortNum));
</script></pre>
***
### 二维数组具体得到数值的方法是Arry[][] 如：
<pre><script>
var scoreStr = "小明:87;小花:81;小红:97;小天:76;小张:74;小小:94;小西:90;小伍:76;小迪:64;小曼:76";
  var scoreArr=[["小明",87],["小花",81],["小红",97],["小天",76],["小张",74],["小小",94],["小西",90],["小伍",76],["小迪",64],["小曼",76]];
  //var scoreArr=scoreStr.split(";");
  var sum=0;
  for(var i=0;i<scoreArr.length;i++){
      //sum+=parseInt(scoreArr[i].substr(scoreArr[i].indexOf(":")+1));
      sum=scoreArr[i][1]+sum;
  };</script></pre>
  ***
## 2017年11月6日
#### clearTimeout(),clearInterval()可以直接在onclick中设置
#### window.history.back()==window.history.go(-1)
#### window.history.forward()==window.history.go(1)
#### location.assign(url) 加载新的页面
#### href="javascript:back()"可以作为标签的属性
### dom操作修改style 如：
<pre><script type="text/javascript">
   var con=document.getElementById("con");
   con.style.color="red";
   con.style.backgroundColor="#ccc";
   con.style.display="none";
  </script></pre>
***
#### document.getElementById() document.getElementsByName() document.getElementsByTagName()
#### 后面两种获取得到的是集合，与数组类似 所以是Elements
***
## 2017年11月7日
### 文本节点单纯是文本，可以用innerHTML访问
### while(x&&x.nodeType!=1){}表示的是当x存在且x.nodeType不为1时
### 写for循环的时候要注意数组的顺序是否会根据循环的变化而变化 如：
<pre><script type="text/javascript">
function clearText() {
  var content=document.getElementById("content");
  // 在此完成该函数
  var cnode=content.childNodes;
  for(i=cnode.length-1;i>0;i--){
      content.removeChild(cnode[i]);
  }
}
</script></pre>
***
## 2017年11月8日
### DOM操作时document不能忘 因为dom操作都要在document(文档)中进行
### <a href="javascript:;"> href里面要完整的JS代码 如window.close();
***
## 2017年11月10日
## 2017年11月11日
## 2017年11月12日
***
## 2017年11月13日
### 条件运算符 如 c?a:b 表示如果c为true,值为a,如果c为false,值为b
***
## 2017年11月14日
### JSON {}
## 2017年11月15日
### arguments是函数的参数，不需要指明名称 如：
<pre>function sayHi() {
  if (arguments[1] == "bye") {
    return;
  }

  alert(arguments[0]);
}</pre>
***
