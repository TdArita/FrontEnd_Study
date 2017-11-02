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
