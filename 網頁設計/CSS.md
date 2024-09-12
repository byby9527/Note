# CSS

### CSS不能單獨使用，必須與HTML或XML一起協同工作。其中，HTML負責確定網頁中有哪些內容，CSS確定以何種外觀(大小、粗細、顏色、對齊和位置)展現這些元素。CSS可以用於設定頁面布局、設定頁面元素樣式、設定適用於所有網頁的全域樣式。

### 範例:
```
body {
  background-color: 顏色; 
}

h1 {
  color: 顏色;
  text-align: 文字對齊的位置;
}

p {
  font-family: 字體;
  font-size: 字體大小;
}
```
### CSS的註解有些時候//這種不能用，通常是C語言才會用，以下例子是CSS常用的註解:
```
  <style>
    /*註解*/
   
    </style>
```

## 主要內容
### CSS由多組「規則」組成。每個規則由「選擇器」（selector）、「屬性」（property）和「值」（value）組成：
### 1.選擇器（Selector）：多個選擇器可以半形逗號（,）隔開。
### 2.屬性（property）：CSS1、CSS2、CSS3規定了許多的屬性，目的在控制選擇器的樣式。
### 3.值（value）：指屬性接受的設定值，多個關鍵字時大都以空格隔開。 屬性和值之間用半形冒號（:）隔開，屬性和值合稱為「特性」。多個特性間用「;」隔開，最後用「{ }」括起來。

---
### 在這個例子中有三個選擇器：p、h2和.highlight，color: red是一個定義，其中color是屬性，red是color的值
```
p{
    font-size: 110%;
    font-family: garamond, sans-serif;
}
h2{
    color: red;
    background: white;
}
.highlight{
    color: red;
    background: yellow;
    font-weight: bold;
}
```
## 選擇器
### 代表去定義id叫什麼名字，id最好是不要重複，id可以去更準確鎖定某一個特定的元素
### 例子
```
#para1 {
  text-align: 位置;
  color: 顏色;
}

```
### class可以套很多次在各種元素上，class代表類別，元素設定類別，就可針對類別來套用，要選擇具有特定類的元素，請輸入句點 (.) 字符，後跟類名。
### 例子
```
.center {
  text-align: 內容位置;
  color: 顏色;
}
<h1 class="center">內容1</h1>
<p class="center">內容2</p> 

```
## 邊框寬度
### 例子:
```
p.one {
  border-style: solid; 
  border-width: 5px;
/*五點*/
}

p.two {
  border-style: solid;
  border-width: medium;
/*中間寬度*/
}

p.three {
  border-style: dotted;
  border-width: 2px;
/*2點*/
}

p.four {
  border-style: dotted;
  border-width: thick;
/*厚的寬度*/
}

```
### 為了縮短代碼，還可以在一個屬性中指定所有單獨的邊框屬性。
### 例子
```
p {
  border: 2px solid green;
}
```
## 填充
### CSS 具有用於指定元素每一側的填充的屬性，可以指定4邊不同的```<Padding>```大小
```
padding-top
padding-right
padding-bottom
padding-left

```
### 或是一個指定，格式為: 上左下右
```
div {
  padding: 25px 50px 75px 100px;
}
```

### 筆記參考網站:[https://www.w3schools.com/html/default.asp](https://www.w3schools.com/html/default.asp)
