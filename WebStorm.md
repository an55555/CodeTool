# 快速生成HTML标签

### 生成带class的标签

div.className => '<div class = "className"></div>'

### 生成带ID的标签

div.IdName => '<div id = "IdName"></div>'

### 生成带属性的标签

div[value=123] => '<div value = "123"></div>'

### 生成带文本内容的标签

div{内容} => `<div>内容</div>`

### 生成一个包含6个p标签的div

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
