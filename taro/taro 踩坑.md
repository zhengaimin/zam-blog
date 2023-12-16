# Image
---
## 图片下方留白
添加样式 `vertical-align:top;` 即可
```html
<Image style="vertical-align:top;" />
```

# 样式
---
- VScode 格式化自动将 `PX` 转为 `px`
	```css
	// 解决方法一
	.style-taro-PX {
	  /* prettier-ignore */
	  font-size: 40PX;
	}
	
	// 解决方法二，文件头部添加，不要添加空格，否则会失效
	/*postcss-pxtransform disable*/



