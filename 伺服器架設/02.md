### ctrl+A 移動到最前面
### ctrl+E 移動到最後面
![](https://hackmd.io/_uploads/H1dyPBiy6.jpg)



### 在伺服器上0.0.0.0代表任意介面
![](https://hackmd.io/_uploads/rkm5PSsy6.jpg)


### 錯誤提示:

![](https://hackmd.io/_uploads/BkkNuHsya.jpg)

## 可由下列步驟來解決:

### 1.檢查server是否正在running
### systemctl status sshd
![](https://hackmd.io/_uploads/SyTypSikp.png)



### 2.檢查port number是否正常
### netstat -tunlp | grep ssh
![](https://hackmd.io/_uploads/ryXgpBoyT.png)


### 3.檢查selinux
### 顯示Disabled就是正確的
![](https://hackmd.io/_uploads/HkJOaBiy6.png)


### 編輯畫面
### 如果編輯完，要輸入rebbot指令重新開機
![](https://hackmd.io/_uploads/Hks_6Hjy6.png)

![](https://hackmd.io/_uploads/HJXITSiJa.png)



### 4.檢查防火牆
![](https://hackmd.io/_uploads/SkNqaBikp.png)


## 使用putty , wincscp 連接到linux vm:


![](https://hackmd.io/_uploads/ByCkRroyT.png)




# 無密碼遠端登入:


### 在linux中.開頭的代表是隱藏檔或是資料夾
### ls -a 顯示所有檔案
![](https://hackmd.io/_uploads/H1yuyLokp.png)

### 產生公鑰和私鑰:
![](https://hackmd.io/_uploads/B11qx8s16.png)

## 最後結果:

![](https://hackmd.io/_uploads/SyWT-Ij1p.png)

### 從7-2的身分退出登入換成7-1:
![](https://hackmd.io/_uploads/Hy6XGLs16.png)

![](https://hackmd.io/_uploads/rkSsMUj16.png)


# 使用scp拷貝檔案和資料夾的練習:

### 拷貝資料:
### 從遠地端拷貝資料到本地端:
![](https://hackmd.io/_uploads/Sy7Pnooka.png)

![](https://hackmd.io/_uploads/r1m7-6s1T.png)

## 安裝tree:
![](https://hackmd.io/_uploads/ryNB-pokp.png)

![](https://hackmd.io/_uploads/Hyev-ai1T.png)

### 拷貝多筆資料:
### touch指令可產生新檔案:
### 在linux中r代表遞迴

![](https://hackmd.io/_uploads/HJW9-6ikp.png)

![](https://hackmd.io/_uploads/BJ03b6oy6.png)


# 改變伺服器的阜號:


## 首先在7-2主機操作:

![](https://hackmd.io/_uploads/BybXVai1a.png)


### 按i可編輯，esc儲存，wq!退出該介面
![](https://hackmd.io/_uploads/HJMENpo1p.png)


### 做完後要重新啟動伺服器:

![](https://hackmd.io/_uploads/r1a8EToJT.png)


![](https://hackmd.io/_uploads/HJge6Npska.png)


## 回到7-1主機來操作:

![](https://hackmd.io/_uploads/HyrwSTska.png)



### 使用ubuntu在安裝軟體或是維護要用apt、apt-get指令

## 期中考必考:
## rpm -qa |grep httpd
### q-->query、a-->all，rpm -qa 查詢linux裡面已安裝多少套件，grep是指過濾器
![](https://hackmd.io/_uploads/SJapOTiJ6.png)

## 期中考必考:
### rpm -qi httpd
### rpm -ql httpd
### rpm -qf /etc/passwd
### 假設誤殺某個檔案，想要從哪個軟體套件就回來，可使用-qf，會告知是從哪裡安裝的
### passwd是從setup軟體套件來的
![](https://hackmd.io/_uploads/B1dt26ik6.png)


![](https://hackmd.io/_uploads/SJp6opiyT.png)


![](https://hackmd.io/_uploads/H1ooTpi16.png)




### 移除套件:
![](https://hackmd.io/_uploads/r1BlRTj1T.png)

