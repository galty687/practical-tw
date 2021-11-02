# CSS 基本介绍

## 什么是CSS

样式语言用于内容的格式呈现。



## CSS语法

`Selector {property1: value1; property2: value2}`



常见写法

```css
selector {
  property1: value1;
  property2: value2;
}
```

例如：

```css
h1 {
	color: blue;
}
```



选择类

```html
<h1 class="big-header">Title</h1>
<a href="index.html">Home</a>
```



`.class-name {property: value}`





```html
<button class="btn btn-1">
  button 1
</button>

<button class="btn btn-2">
  button 2
</button>

<button class="btn btn-3">
  button 3
</button>
```



```css
.btn {
  padding: 10px;
  color: white;
}

.bth-1 {background-color: green}
.bth-2 {background-color: blue}
.bth-3 {background-color: purple}
```



```css
#id {
  property: value;
}
```



```css
selector1.selector-2 {

	property: value;

}
```



```html
<h1 class="large-heading">Title</h1>
```



```css
h1.large-header {
  font-size: 200%
}
```



```html
<h2 id="big-blue" class="large blue">Title</h2>
```

```
#big-blue.large.blue
```

 