####jQuery hide() 和show()
**使用hide()和show() 可以实现HTML 元素的隐藏和显示**   
语法：  
*$(selector).hide(speed,callback);*  
*$(selector).show(speed,callback);*  
可选的 speed 参数规定隐藏/显示的速度，可以取以下值："slow"、"fast" 或毫秒。  
可选的 callback 参数是隐藏或显示完成后所执行的函数名称。  


<!-- lang:javascript-->
	$(document).ready(
				function(){
					$("p").click(
							 function(){
						 			$(this).hide();
  									    }
								);
						}
					);

####jQuery toggle() 
 **使用toggle() 方法可以切换hide()和show() 方法，显示被隐藏元素or隐藏已显示元素**：  
 语法：  
 *$(selector).toggle(speed,callback);*  
可选的 speed 参数规定隐藏/显示的速度，可以取以下值："slow"、"fast" 或毫秒。  
可选的 callback 参数是 toggle() 方法完成后所执行的函数名称。

<!-- lang:javascript-->
    $(document).ready(function(){
      $("button").click(function(){
		  $("p").toggle("slow");
		  });
		});