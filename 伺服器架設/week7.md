## 透過wifi連線ipv6:



## VMware 設定:

![](https://hackmd.io/_uploads/SJwBsCVzT.jpg)


### Edit->virtual Network editor




## VirtualBox 設定:


![](https://hackmd.io/_uploads/S1n8_PIzp.png)






### 先到cmd去ping一下自己的ip位址
![](https://hackmd.io/_uploads/HyVzrDUMT.png)





### 如果出現錯誤顯示could not reslove host....，表示名稱解析有問題
### 解決辦法: vim /etc/resolv.conf去編輯dns，並改成8.8.8.8

![](https://hackmd.io/_uploads/H1yy5DLf6.png)



![](https://hackmd.io/_uploads/H1Ql5DLf6.png)



### 啟動伺服器:

![](https://hackmd.io/_uploads/BJDkiDLMp.png)









## 最後結果:

### 連線方式: [ipv6的ip]/milk.htm，記得ipv6是2001開頭
![3](https://hackmd.io/_uploads/rJ3fMYSLp.png)


![](https://hackmd.io/_uploads/Syo0S_UM6.png)


### 到這個網站:https://dynv6.com/



![](https://hackmd.io/_uploads/HywHv_Lza.png)


![](https://hackmd.io/_uploads/ByyLwd8Gp.png)


## 要到信箱去做確認:

![](https://hackmd.io/_uploads/SJ_vw_LzT.png)



![](https://hackmd.io/_uploads/H1M5DdLGT.png)




## 最後結果:

![](https://hackmd.io/_uploads/SJ9euOIfT.png)




### wifi ipv6:
2001:b400:e758:93cf:4561:47e:e1b9:18e1





## cp指令用於拷貝用，加上-i 就是用來詢問，拷貝過去的檔案如果已存在，就會去做詢問，每次執行cp都是在執行cp -i，意思就是把完整指令(cp -i)重新設計另一個別名給cp
![](https://hackmd.io/_uploads/By-kou8M6.png)

## 加上\ 就是還原:

![](https://hackmd.io/_uploads/SJLrnd8fa.jpg)


## 如果要編輯alias，在其他視窗或是行程都可開啟，可以使用 vim .bashrc

![](https://hackmd.io/_uploads/S1cYJYIf6.png)


## 輸入source .bashrc 或是 . .bashrc

![](https://hackmd.io/_uploads/SyTGetLza.png)




## 當中的設定會套用到所有使用者
![](https://hackmd.io/_uploads/BJScWK8zp.jpg)

## 如果是自己的配置,修改檔案室自身目錄下的.bashrc，如果希望套用到整個系統的使用者,修改的檔案是/etc/profile,記得要用root


![](https://hackmd.io/_uploads/SJH2zYLfa.png)



![](https://hackmd.io/_uploads/B13nfKLGa.png)





![](https://hackmd.io/_uploads/r19y7FIzp.png)

![](https://hackmd.io/_uploads/B1axQK8z6.jpg)

### 加上-e  \t會變成tab鍵
![](https://hackmd.io/_uploads/BJevmtIzT.jpg)



### su -tom 切換成tom使用者 ，echo $HOME 顯示user的家目錄
![](https://hackmd.io/_uploads/rk7imK8fT.jpg)




![](https://hackmd.io/_uploads/BJofVFIz6.jpg)


## PATH最主要的目的是如果要執行一個指令，就需要打相對路徑或是絕對路徑，解決方法是可以去編輯vim .bashrc並輸入以下內容，這樣就不需要打./(相對路徑或是絕對路徑)，直接打檔案名稱就可以執行
![](https://hackmd.io/_uploads/BkjVEt8zp.jpg)


![](https://hackmd.io/_uploads/SJWUNFUMa.jpg)


![](https://hackmd.io/_uploads/SyjXStLGp.jpg)


## 2個指令用途都是顯示使用者帳號
![](https://hackmd.io/_uploads/Byg4HK8za.jpg)



### 產生1-10:
![](https://hackmd.io/_uploads/S1Iz4DUfp.png)


### 如果要進行取代可以使用tr指令
