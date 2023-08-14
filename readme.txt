这是单开版随机数的js代码
=======================
	  <script>
function RandomPick(){
	var x=document.getElementById("randomMathjs")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
</script>
这是双开版的
=======================
	  <script>
function RandomPick(){
	var x=document.getElementById("randomMathjs")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
function RandomPicksec(){
	var x=document.getElementById("randomMathsec")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
</script>
===========================================================================
html（已经把样式表等去除）
双开版：

<!DOCTYPE html>
<html>
<head>
	<style>
		h1 {
			font-size:80px;
		}
	</style>
  <title>Bootstrap5 随机数</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">

</head>
<body>

<div class="container mt-3">
  <div align="center" class="card">
    <div class="card-header">随机数3.0.0</div>
    <div class="card-body">
	  <nav>
  <a href="./单开.html">单开</a> |
  <a>双开</a> |

</nav>
	 <hr>
		<p>您现在使用的是：双开模式</p>
	  <div class="card">
  <div align="center" class="card-body">
		  
		  
	  <h1 id="randomMathjs">第一个人未抽取</h1>	
	  <hr>
	  <h1 id="randomMathjssecdary">第二个人未抽取</h1>
	   <div class="btn-group btn-group-lg">
		   
    <button onclick="RandomPick()" type="button" class="btn btn-primary">抽取第一个人</button>
    <button onclick="RandomPicksec()" type="button" class="btn btn-primary">抽取第二个人</button>

  </div>
	  <script>
function RandomPick(){
	var x=document.getElementById("randomMathjs")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
function RandomPicksec(){
	var x=document.getElementById("randomMathjssecdary")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
</script>
		  </div>
</div>
	  </div>
	  <div align="center">
	  <img src="./jian.jpeg" width="300" height="200" alt="肥肠抱歉，图没了">
	</div> 
    <div class="card-footer">本人保证所有随机数结果的公正性</div>
  </div>
</div>

</body>
</html>
单开版：
<!DOCTYPE html>
<html>
<head>
	<style>
		h1 {
			font-size:80px;
		}
	</style>
  <title>Bootstrap5 随机数</title>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
 
</head>
<body>

<div class="container mt-3">
  <div align="center" class="card">
    <div class="card-header">随机数3.0.0</div>
    <div class="card-body">
	  <nav>
  <a>单开</a> |
  <a href="./双开.html">双开</a> |

</nav>
	 <hr>
		<p>您现在使用的是：单开模式</p>
	  <div class="card">
  <div align="center" class="card-body">
		  
		  
	  <h1 id="randomMathjs">请先抽取</h1>	
	   <button type="button" onclick="RandomPick()" class="btn btn-outline-primary">抽一个人</button>
	  <script>
function RandomPick(){
	var x=document.getElementById("randomMathjs")
	x.innerHTML=Math.floor((Math.random()*30)+1);
}
</script>
		  </div>
</div>
	  </div>
	  <div align="center">
	  <img src="./jian.jpeg" width="300" height="200" alt="肥肠抱歉，图没了">
	</div> 
    <div class="card-footer">
		
		本人保证所有随机数结果的公正性</div>
  </div>
</div>

</body>
</html>
==========================
我拿人头保证公正性！！！
随机数3.00 
==========================
bug （特性）
已知：
暂时没有啥
==========================
js代码注释
innerHTML=Math.floor((Math.random()*30)+1);
            ||   ||                 ||
            \/   \/                 \/
     js自带的Math  不出现小数点后x位  从1（这就是为啥后面有+1）~30中抽取