####jQuery stop()方法用于在动画或效果完成前对它们进行停止
----
**stop() 方法适用于所有 jQuery 效果函数，包括滑动、淡入淡出和自定义动画。**   
语法  
*$(selector).stop(stopAll,goToEnd);*  
可选的 stopAll 参数规定是否应该清除动画队列。默认是 false，即仅停止活动的动画，允许任何排入队列的动画向后执行。  
可选的 goToEnd 参数规定是否立即完成当前动画。默认是 false。  
因此，默认地，stop() 会清除在被选元素上指定的当前动画。  
<!--lang:javaStript--!>
	$("#stop").click(function(){  
	  $("#panel").stop();  
	});  
