# JavaScript





## 編程
---
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
