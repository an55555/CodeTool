# 快速生成HTML标签

### 快速生成HTML结构

!加TBG键

```html
<!doctype html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport"
          content="width=device-width, user-scalable=no, initial-scale=1.0, maximum-scale=1.0, minimum-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

### 生成带class的标签

p.className => `<p class = "className"></p>`

**如果生成是DIV，直接.classNam即可**

### 生成带ID的标签

p.IdName => `<p id = "IdName"></p>`

**如果生成是DIV，直接#IdName即可**

### 生成带属性的标签

div[value=123 tab=myTag] => `<div value = "123" tab = "Mytag"></div>`

### 生成带文本内容的标签

div{内容} => `<div>内容</div>`

### 生成子标签：一个包含6个p标签的div

div>p*6 => 

```htlm
<div>
  <p></p>
  <p></p>
  <p></p>
  <p></p>
  <p></p>
  <p></p>
</div>
```

### 生成兄弟标签

div+p+div =>

```html
<div><div>
<p></p>
<div></div>
```

### 生成上级元素：即包含子元素又能有同级元素

div>ul>li^div =>

```html
<div>
  <ul>
  <li></li>
  <ul></ul>
  <div></div>
</div>
```

**一个`^`表示往上跳一层**

### 分组()

(div>dl>(dt+dd)*3)+footer>p => 

```html
<div>
    <dl>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
        <dt></dt>
        <dd></dd>
    </dl>
</div>
<footer>
    <p></p>
</footer>
```

### 连续序号标签

ul>li.item$*5 =>

```html
<ul>
 <li class="item1"></li>
 <li class="item2"></li>
 <li class="item3"></li>
 <li class="item4"></li>
 <li class="item5"></li>
</ul>
```

指定位数 ul>li.item$$$*5 =>

```html
<ul>
    <li class="item001"></li>
    <li class="item002"></li>
    <li class="item003"></li>
    <li class="item004"></li>
    <li class="item005"></li>
</ul>
```

倒序 ul>li.item$@-*5 =>

```html
<ul>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
    <li class="item2"></li>
    <li class="item1"></li>
</ul>
```

指定开始的序号 ul>li.item$@3*5

```html
<ul>
    <li class="item3"></li>
    <li class="item4"></li>
    <li class="item5"></li>
    <li class="item6"></li>
    <li class="item7"></li>
</ul>
```

ul>li.item$@-3*5

```html
<ul>
    <li class="item7"></li>
    <li class="item6"></li>
    <li class="item5"></li>
    <li class="item4"></li>
    <li class="item3"></li>
</ul>
```

## 常用缩写

a => `<a href=""></a>`

br => `</br>`

更多 https://www.w3cplus.com/tools/emmet-cheat-sheet.html
