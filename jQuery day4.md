####jQuery 滑动方法可使元素上下滑动。
----
jQuery 拥有以下滑动方法：  
* slideDown()   
* slideUp()  
* slideToggle()  
**jQuery slideDown() 方法用于向下滑动元素**
语法：  
*$(selector).slideDown(speed,callback);*  
可选的 speed 参数规定效果的时长。它可以取以下值："slow"、"fast" 或毫秒。  
可选的 callback 参数是滑动完成后所执行的函数名称  
<!-- lang:javascript-->  
	$("#flip").click(function(){  
	  $("#panel").slideDown();  
	});  
**jQuery slideUp() 方法用于向上滑动元素。**  
语法：  
*$(selector).slideUp(speed,callback);*  
**jQuery slideToggle() 方法可以在 slideDown() 与 slideUp() 方法之间进行切换。**  
如果元素向下滑动，则 slideToggle() 可向上滑动它们。  
如果元素向上滑动，则 slideToggle() 可向下滑动它们。  
*$(selector).slideToggle(speed,callback);*