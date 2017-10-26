# 这是我在学习JavaScript中遇到的问题和相应的解决方案
## 2017年10月19日
###  在Alert中实现换行 例如：
<pre><script type="text/javascript">
  var mya,mya2;
  mya=5;
  mya2=15;
  alert("mya的值是:"+mya+"\n"+"mya2的值是:"+mya2);
</script></pre>
## 2017年10月20日
### ==(是否相等)是比较操作符 !=(是否不等)是比较操作符，输出true或false(不是1或者0)
## <2017年10月26日>
### for循环中用;符号分隔条件不要用成逗号"," 例如:
<pre>
<script type="text/javascript">
var myarr=new Array();
for(var i=0;i<3;i++){
    myarr[i]=new Array();
    for(var j=0;j<6;j++);
    myarr[i][j]=i*j;
}
document.write("第三行第六个数组值为:"+myarr[2][5]);
</script>
</pre>
