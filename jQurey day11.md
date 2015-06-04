####jQuery设置 text()、html() 以及 val()
----

> * text() - 设置或返回所选元素的文本内容
> * html() - 设置或返回所选元素的内容（包括 HTML 标记）
> * val() - 设置或返回表单字段的值> 
```$("#btn1").click(function(){
  $("#test1").text("Hello world!");
});
$("#btn2").click(function(){
  $("#test2").html("<b>Hello world!</b>");
});
$("#btn3").click(function(){
  $("#test3").val("Dolly Duck");
});```    

**text()、html() 以及 val() 的回调函数**  
上面的三个 jQuery 方法：text()、html() 以及 val()，同样拥有回调函数。回调函数由两个参数：被选元素列表中当前元素的下标，以及原始（旧的）值。然后以函数新值返回您希望使用的字符串。   
	
```$("#btn1").click(function(){
  $("#test1").text(function(i,origText){
    return "Old text: " + origText + " New text: Hello world!
    (index: " + i + ")";
  });
});```

```$("#btn2").click(function(){
  $("#test2").html(function(i,origText){
    return "Old html: " + origText + " New html: Hello <b>world!</b>
    (index: " + i + ")";
  });
});```    

**设置属性 - attr()**  
jQuery attr() 方法也用于设置/改变属性值。  
```$("button").click(function(){
  $("#w3s").attr({
    "href" : "http://www.w3school.com.cn/jquery",
    "title" : "W3School jQuery Tutorial"
  });
});```   
**attr() 的回调函数**   
jQuery 方法 attr()，也提供回调函数。回调函数由两个参数：被选元素列表中当前元素的下标，以及原始（旧的）值。然后以函数新值返回您希望使用的字符串。	
```$("button").click(function(){   
  $("#w3s").attr("href", function(i,origValue){   
    return origValue + "/jquery";   
  });
});```	

