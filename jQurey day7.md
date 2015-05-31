####jQuery Callback 函数在当前动画 100% 完成之后执行
----
由于 JavaScript 语句（指令）是逐一执行的 - 按照次序，动画之后的语句可能会产生错误或页面冲突，因为动画还没有完成。
为了避免这个情况，您可以以参数的形式添加 Callback 函数。  
典型的语法：  
*$(selector).hide(speed,callback)*
<!--lang:javaScript--!>
	$("p").hide(1000,function(){  
	alert("The paragraph is now hidden");  
	});  