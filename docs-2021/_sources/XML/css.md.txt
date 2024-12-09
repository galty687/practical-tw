# CSS 基本介绍

## 什么是CSS

样式语言用于内容的格式呈现。

### 需要掌握的内容：

### 单个

1. 选择元素
2. 选择类
3. 选择 id

### 组合
1.  .ancestor . child {property: value}
2.  element.class child-element
3.  element child-element
4. 

## CSS语法

`Selector {property1: value1; property2: value2}`



### 选择元素

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



### 选择“类”

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

### 选择 id

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

参考资源
- [CSS Reference ](https://cssreference.io)
- [Color Converter](https://www.w3schools.com/colors/colors_converter.asp)
- [PrintCSS Playground](https://printcss.live/)