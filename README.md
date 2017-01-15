# dataBirthdayJquery
一个jquery的生日选择插件，不是select形式,被ui逼的～～
#用法:
### 首先提供1个带定位属性的div包住input框，方便控件根据此div定位
   <pre>
  &lt;div class="div_input" style="position: relative;"&gt;
			&lt;input type="text" name="" id="dataInput" value="" /&gt;			
  &lt;/div&gt;
   </pre>

###脚本调用方式：大部分我都内置在组件中了,外面只暴露了1个接口，方便调节位置
```javascript
$("#dataInput").off("timeData").on("timeData",function(event){
	console.log("回调函数")//这个是组件消失之后的回调，如果有需要可以处理用户自己的逻辑	
}).dataYear({
	dataTop:20   //这20是根据input定位的位置，可以自定义配置
})

###控件样式，如果大家觉得slect样式难看，这种也未尝不是一个好方式
![github](https://santant.github.io/githubImg/jquery-data.png "github") 
