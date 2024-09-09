## site to site 用於企業的VPN


## 配置PPTP VPN服務端到客戶端的連接:

## 參考: https://help.aliyun.com/zh/ecs/how-do-i-configure-a-connection-between-a-pptp-vpn-server-and-a-pptp-vpn-client-on-a-centos-7-instance


## centos7-1: 設定--網路:
### 需要配置3張網路卡:
![10](https://hackmd.io/_uploads/Bk3cUQzNp.png)
![11](https://hackmd.io/_uploads/SJei87MNp.png)
![12](https://hackmd.io/_uploads/ryEoU7fVa.png)


## centos7-2 只需配置1張網路卡:
![13](https://hackmd.io/_uploads/HJ8C8QfEa.png)



## 到7-1主機操作流程:

### ip設置:
![15](https://hackmd.io/_uploads/S1AAumfVa.png)

![16](https://hackmd.io/_uploads/By4xY7G46.png)

## 7-2:
![17](https://hackmd.io/_uploads/S1-GKmfNT.png)


##  回到7-1操作:
###  安裝此指令:
![14](https://hackmd.io/_uploads/SkbyOXzEp.png)


### 輸入此指令
![18](https://hackmd.io/_uploads/BJFRF7zVa.png)

### 會顯示這些內容並修改:
![19](https://hackmd.io/_uploads/ryV-57fVT.png)

### 如果沒有顯示內容，請執行此指令: yum install -y epel-release


### 輸入此指令:
![20](https://hackmd.io/_uploads/SkR0qXf4T.png)

### 會顯示這些內容並修改:
![21](https://hackmd.io/_uploads/SJhks7MNa.png)


### 輸入此指令:
![22](https://hackmd.io/_uploads/SJDLoQzE6.png)

### 會顯示這些內容並修改:
![23](https://hackmd.io/_uploads/rk2PsQG46.png)


### 輸入此指令:
![24](https://hackmd.io/_uploads/rJLRimz4p.png)


### 會顯示這些內容並修改:
![25](https://hackmd.io/_uploads/rJxpynmzNa.png)



### 輸入此指令:
![26](https://hackmd.io/_uploads/ByZInmGNa.png)

### 會顯示這些內容並修改:
![27](https://hackmd.io/_uploads/S17v3XzN6.png)


### 輸入此指令與及其結果:

![28](https://hackmd.io/_uploads/Syy3nQz4p.png)


### 重新啟動指令:
![29](https://hackmd.io/_uploads/rkHX67GNa.png)

### 設定--網際網路--vpn:
![30](https://hackmd.io/_uploads/rJC51NzEp.png)

### 到命令提示字元(cmd)測試 ping7-1主機:
### 最後結果:
![31](https://hackmd.io/_uploads/Hk16JVMN6.png)
![32](https://hackmd.io/_uploads/HywpJVGN6.png)

![33](https://hackmd.io/_uploads/ByKJx4fEp.png)

