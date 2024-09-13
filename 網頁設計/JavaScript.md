# JavaScript

## 物件與JSON:
大括號會形成一個物件，定義一個物件，可以透過名字來取得內容
### 例子:
```
VAR bbb={ name:'bbb', age:18}

```
## 可以內嵌在網頁裡面，點下按鈕就會顯示目前的時間
### document是指整個網頁，getElementById指希望可以從網頁裡取得一個節點，本程式取得的節點是id="demo"，並且把innerHTML塞入Date()裡，Date()的時間會轉成字串並顯示其時間。
### 例子:
```
<button type="button"
onclick="document.getElementById('demo').innerHTML = Date()">內容</button>
<p id="demo></p>"
```
## 跨網站指令碼 (Cross-site scripting):
### 是一種網站應用程式的安全漏洞攻擊，是代碼注入的一種。它允許惡意使用者將程式碼注入到網頁上，其他使用者在觀看網頁時就會受到影響。這類攻擊通常包含了HTML以及使用者端手稿語言。

---
## JavaScript 可以以不同的方式顯示數據:
```
1.寫入 HTML 元素innerHTML。
2.寫入 HTML 輸出document.write()。
3.寫入警報框window.alert()。
4.寫入瀏覽器控制台console.log()。
```

---
## 可以做加法運算，該id屬性定義 HTML 元素。該innerHTML 屬性定義了 HTML 內容
### 例子:
```
<p id="demo"></p>
<script>
document.getElementById("demo").innerHTML = 1+ 1;
</script>
```
---

## 使用 document.write()，但是要注意在加載 HTML 文檔後使用 document.write() 將刪除所有現有的 HTML
### 例子:
```
<script>
document.write(1 + 1);
</script>
```
---

## 使用警報框來顯示數據
### 例子:
```
<script>
window.alert(1 + 1);
</script>
```

---

## console.log()有個缺點是在畫面上看不到，但可以到右上角的更多工具-->開發人員工具，就可以看到了，因此使用這個方法是為了在開發人員工具這邊看到
### 例子:
```
<script>
console.log(1 + 1);
</script>
```

---

## 4種變數的宣告
### 使用var是會回朔，在後面宣告，前面就可以用，但僅限於同一層的前面。使用let是從宣告開始，變數才可以用，使用const是宣告後不能更改，改掉會產生錯誤。完全不宣告(nothing)是var x = 5;這樣，代表這個變成全義變數
```
1.Using var

2.Using let

3.Using const

4.Using nothing
```

## Strings:
### let text= ' It 's alright.'; 這是單引號，但如果是雙引號，可以省略\，let text= "It 's alright.";
### 例子:
```
<p id="demo"></p>
<script>
let text = 'It\'s alright.';
document.getElementById("demo").innerHTML = text; 
</script>
```
---

### 使用==運算符時，型態不相等，值相等就可以，但使用===運算符時，型態和值都要相等，一般在JavaScript判斷相等都會用===運算，因為==運算會跨型態的相等
### 例子:
```
<p id="demo"></p>
<script>
let x = "dog";        
let y = new String("dog"); 
document.getElementById("demo").innerHTML = (x==y);
</script>
```
---

### slice(start, end):把其中一小段抽出來，從起點抽到終點 ，substring(start, end)、substr(start, length)也和slice是一樣的。
### 例子:
```
<p id="demo"></p>
<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.slice(7,13); 
</script>
```
### 執行結果:Banana

---

### 如果省略第二個參數，該方法將切出字符串的其餘部分，不寫後面就將整個後面抽出來
### 例子:
```
<p id="demo"></p>
<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.slice(7);
</script>
```
### 執行結果:Banana,Kiwi

---

### substring()類似於slice()，不同之處在於substring()不能接受負索引
### 例子:
```
<p id="demo"></p>
<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.substring(7,13);
</script>
```
### 執行結果:Banana

---

### substr()不同之處在於第二個參數指定 提取部分的長度
### 例子:
```
<p id="demo"></p>
<script>
let str = "Apple, Banana, Kiwi";
document.getElementById("demo").innerHTML = str.substr(7,6);
</script>
```
---

### concat()可以使用該方法代替加號運算符，這兩行的作用相同
### 例子:
```
text = "Hello" + " " + "World!";

text = "Hello".concat(" ", "World!");

```

---

### 以下例子是檢查輸入。如果值錯誤，則拋出異常 (err)，異常 (err) 被 catch 語句捕獲並顯示自定義錯誤消息:
```
<input id="demo" type="text">
<button type="button" onclick="myFunction()">Test Input</button>
<p id="p01"></p>
<script>
function myFunction() {
  const message = document.getElementById("p01");
  message.innerHTML = "";
  let x = document.getElementById("demo").value;
  try { 
    if(x == "")  throw "empty";
    if(isNaN(x)) throw "not a number";
    x = Number(x);
    if(x < 5)  throw "too low";
    if(x > 10)   throw "too high";
  }
  catch(err) {
    message.innerHTML = "Input is " + err;
  }
}
</script>
```



---

## 編程

JavaScript是一種手稿語言，其原始碼在發往客戶端執行之前不需經過編譯，而是將文字格式的字元代碼發送給瀏覽器由瀏覽器解釋執行。直譯語言的弱點是安全性較差，而且在JavaScript中，如果一條執行不了，那麼下面的語言也無法執行。而其解決辦法就是於使用例外處理try {} catch () {}︰
### 範例:
```
console.log("a");  //這是正確的
console.log("b");  //這是正確的
console.logg("c"); //這是錯誤的，並且到這裡會停下來
console.log("d");  //這是正確的
console.log("e");  //這是正確的

/* 解決辦法 */
try { console.log("a"); } catch (e) {}  //這是正確的
try { console.log("b"); } catch (e) {}  //這是正確的
try { console.logg("c"); } catch (e) {} //這是錯誤的，但是到這裡不會停下來，而是跳過
try { console.log("d"); } catch (e) {}  //這是正確的
try { console.log("e"); } catch (e) {}  //這是正確的
```



### 筆記參考網站:[https://www.w3schools.com/js/default.asp](https://www.w3schools.com/js/default.asp)
