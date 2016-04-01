# css 盒子模型


1. 当我们放置一个块级元素于页面上时，并且不设置它的定位属性（relative，absolute，fixed），即position:static，或者设置了position:relative的情况下，块的宽度是延伸自动填充满它的父元素的宽度区域。所以当我们在计算一个被包裹中的元素的宽度时，我们只需要用父元素减去这个元素的外边距，边框，内边距，和scrollbar，剩下就是它的宽度，因为它会自动填充。

        
		.box1{
			background:black;
			color:White;
        	height:100px;
        	padding:10px;
        	border:20px solid Red;
        	margin:30px;             
    	}
		<div class="box1">For static or absolutely relative</div>

![块的宽度自动填充整个父元素][1]

  
[1]: ff.png
  
