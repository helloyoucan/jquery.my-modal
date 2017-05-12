# jquery.my-modal
一个modal的jq插件
---
浏览器支持：IE9+
---
### 有默认风格和win风格

#### 调用方式

```javascript
<script type="text/javascript" src="js/jquery1.9.min.js"></script>
<script type="text/javascript" src="js/jquery.my-modal.1.1.js"></script>
<script>
	var m1 = new MyModal.modal(function() {
		alert("你点击了确定");//点击确定后的回调函数
	});
	$('.btn1').on("click", function() {
		m1.show();//显示
		/*隐藏的方法*/
		//m1.hide()
	});
</script>
```

#### 默认风格

![默认风格](http://opok8iwaa.bkt.clouddn.com/image/github/modal/defaultStyle.jpg)

#### win风格

![win风格](http://opok8iwaa.bkt.clouddn.com/image/github/modal/winStyle.jpg)

#### Html模板

```html
<button class="btn1">open the modal</button>
<div class="m-modal">
	<div class="m-modal-dialog">
		<div class="m-top">
			<h4 class="m-modal-title">
				标题
			</h4>
			<span class="m-modal-close">&times;</span>
		</div>
		<div class="m-middle">
		<!--content-->
			<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta facere repellat culpa similique officiis praesentium eos! Eum atque maxime beatae similique nihil perferendis laborum tempora amet adipisci corrupti. Porro id.</p>
			<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dicta facere repellat culpa similique officiis praesentium eos! Eum atque maxime beatae similique nihil perferendis laborum tempora amet adipisci corrupti. Porro id.</p>
		</div>
		<div class="m-bottom">
			<button class="m-btn-sure">确定</button>
			<button class="m-btn-cancel">取消</button>
		</div>
	</div>
</div>
```

