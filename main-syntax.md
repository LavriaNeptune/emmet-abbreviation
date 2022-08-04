## 元素标签简写

书写标签名生成对应的 HTML 标签...非标准标签名也可以生成对应标签，这是考虑到某些框架的自定义组件的使用情形。

`div` -> `<div></div>`

## 插入文字节点：`{}`

p{Hello World} 表示：

```HTML
<p>Hello World</p>
```

## 元素关系符号

### 子节点关系：`>`

`div>p` 表示：

```HTML
<div>
  <p></p>
</div>
```

### 相邻节点：`+`

div+p 表示：

```HTML
<div></div>
<p></p>
```

### 上层节点：`^`

div>p>span^div 表示：

```HTML
<div>
  <p><span></span></p>
  <div></div>
</div>
```

`^` 可以存在复数个，表示跳跃的层级。

### 复数节点 `*n`

`ul>li*3` 表示：

```HTML
<ul>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

### 组合节点 `()`

将一组节点视为单个节点，只需要通过小括号将之包裹即可...

## 元素属性简写

### 添加 id 属性: `#`

`div#test` 表示：

```HTML
<div id="test"></div>
```

### 添加 class 属性: `.`

div.hello

```HTML
<div class="hello"></div>
```

### 添加自定义属性: `[]`

`div[data="myData"]` 表示：

```HTML
<div data="myData"></div>
```
