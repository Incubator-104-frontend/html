# Practice for HTML tag

## 結構類(Structure)

### `<html>`

  HTML 文件的開始及結束

### `<head>`

  提供 HTML 會使用到的 Meatdata，包含 Javascript, CSS
  
### `<body>`

  所有內容都包在這裡
  
## 容器類(Container)

### `<h1> - <h6>`

  章節標題，數字越大的標題會越來越小，最多到第六層
  
``` html
<h1>This is H1</h1>
<h2>This is H1</h2>
<h3>This is H1</h3>
<h4>This is H1</h4>
<h5>This is H1</h5>
<h6>This is H1</h6>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/h1toh6.html](https://incubator-104-frontend.github.io/html/roy.wu/src/h1toh6.html)

### `<p>`

  章節段落
  
``` 
<h1>The H1 tag</h1>
<p>The p tag<p>
<h2>The H2 tag</h2>
<p>The p tag</p>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/p.html](https://incubator-104-frontend.github.io/html/roy.wu/src/p.html)

### `<div>`

  本身沒有任何意義，但可以把任意物件框起來，加上 `class` 和 `id` ，日後 selector 選取的時候比較方便！
  
```
<div>
  <p>Hello World!</p>
</div>
<div>
  <p>How are you?</p>
</div>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/div.html](https://incubator-104-frontend.github.io/html/roy.wu/src/div.html)

### `<span>`

  和 `div` 類似本身是沒有意義的，但 `span` 專門框 in-line 物件
  
```
<span>
  <p>This is first attempt to use span</p>
</span>
<span>
  <p>And This a second time</p>
</span>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/span.html](https://incubator-104-frontend.github.io/html/roy.wu/src/span.html)


### `<em>`

  強調重點，支援巢狀結構，通常瀏覽器會以斜體表示，越深層表示越重要
  
```
<p>
  Mary and Kelly earned <em>$5000</em> this morning
</p>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/em.html](https://incubator-104-frontend.github.io/html/roy.wu/src/em.html)


### `<strong>`

  強調重點，通常會以粗體表示
  
```
<p>
  What date is <strong>today</strong>?
</p>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/strong.html](https://incubator-104-frontend.github.io/html/roy.wu/src/strong.html)

### `<a>`

  超連結，搭配 `href` 使用
  
```
<a href="https://github.com/Incubator-104-frontend/html">Github repo</a>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/a.html](https://incubator-104-frontend.github.io/html/roy.wu/src/a.html)


### `<ol>` `<ul>` `<li>`

  ol: 有順序的清單(Order list) <br>
  ul: 沒順序的清單(Unorder list) <br>
  都搭配 `<li>` (List item) 使用
  
```
<ol>
  <li>Honda</li>
  <li>Toyota</li>
  <li>Nissan</li>
<ol>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/ol.html](https://incubator-104-frontend.github.io/html/roy.wu/src/ol.html)
 
```
<ul>
  <li>Honda</li>
  <li>Toyota</li>
  <li>Nissan</li>
<ul>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/ul.html](https://incubator-104-frontend.github.io/html/roy.wu/src/ul.html)

## 表單類(Tables)

### `<table>` `<th>` `<tr>` `<td>`

  table: 宣告表單區塊 <br>
  th: 標頭(Table header) <br>
  tr: 行(Table row) <br>
  td: 元素 
  
```
<table>
  <tr>
    <th>ID</th>
    <th>Name</th>
    <th>Score</th>
  </tr>
  <tr>
    <td>1</td>
    <td>Mike</td>
    <td>A</td>
  </tr>
  <tr>
    <td>2</td>
    <td>Jack</td>
    <td>A+</td>
  </tr>
</table>
```
[https://incubator-104-frontend.github.io/html/roy.wu/src/table.html](https://incubator-104-frontend.github.io/html/roy.wu/src/table.html)

參考資料: [MDN: HTML elements reference](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)