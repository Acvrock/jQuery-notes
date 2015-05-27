###jQurey效果－淡入淡出
----
jQurey拥有4种fade方法：   
* fadeIn()  
* fadeOut()  
* fadeToggle()  
* fadeTo()   

----
**jQuery fadein()用于淡入已隐藏元素**  
语法：  
*$(selector).fadeIn(speed,callback);*  
可选的 speed 参数规定效果的时长。它可以取以下值："slow"、"fast" 或毫秒。  
可选的 callback 参数是 fading 完成后所执行的函数名称。  

<!-- lang:javascript-->   
		$("button").click(function(){    
	    $("#div1").fadeIn();    
	    $("#div2").fadeIn("slow");   
 	    $("#div3").fadeIn(3000);   
		});   

**jQuery fadeOut() 方法用于淡出可见元素。**  
语法：  
*$(selector).fadeOut(speed,callback);*  
**jQuery fadeToggle() 方法可以在 fadeIn() 与 fadeOut() 方法之间进行切换。**  
如果元素已淡出，则 fadeToggle() 会向元素添加淡入效果。    
如果元素已淡入，则 fadeToggle() 会向元素添加淡出效果。  
语法：  
*$(selector).fadeToggle(speed,callback);*  
**jQuery fadeTo() 方法允许渐变为给定的不透明度（值介于 0 与 1 之间）。**  
语法：  
*$(selector).fadeTo(speed,opacity,callback);*   
fadeTo() 方法中必需的 opacity 参数将淡入淡出效果设置为给定的不透明度（值介于 0 与 1 之间）。  
<!-- lang:javascript-->   
	  $("button").click(function(){  
	  $("#div1").fadeTo("slow",0.15);  
	  $("#div2").fadeTo("slow",0.4);  
	  $("#div3").fadeTo("slow",0.7);  
	});     

 