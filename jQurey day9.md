####jQuery - 获得内容和属性
----
**jQuery DOM 操作**  
*获得内容 - text()、html() 以及 val()*  
三个简单实用的用于 DOM 操作的 jQuery 方法：  
text() - 设置或返回所选元素的文本内容  
html() - 设置或返回所选元素的内容（包括 HTML 标记）  
val() - 设置或返回表单字段的值  
<!--lang:javaScript--!>
	$("#btn1").click(function(){  
  alert("Text: " + $("#test").text());  
});  
$("#btn2").click(function(){  
  alert("HTML: " + $("#test").html());  
});  
	$("#btn1").click(function(){	
    alert("Value: " + $("#test").val());  
  });    
  
 ----
  *获取属性 - attr()*  
jQuery attr() 方法用于获取属性值。  
<!--lang:javaScript--!>
	$("button").click(function(){  
  alert($("#w3s").attr("href"));  
});  
 