# 如何完全刪除github的檔案，目的是怕侵權:

### 1.先到網路上搜尋git download，並點選 Download -Git SCM


### 2.點選自己使用的平台(Winodw 、macOS 、Linux/Unix)並下載


### 3.安裝中記得勾選git bash，自動勾選就不用再勾選了


### 4.開啟Visual Studio Code，到終端機旁邊會看到一個加號的符號旁邊的下拉式選單點選bash，並打開


### 5.但如果是剛安裝要先重開一次Visual Studio Code


### 6.在bash環境中的指令輸入git，如果有顯示usage，就表示安裝好，否則就是失敗


### 7.到github的頭像下拉式選單中的Settings，點ssh and gpg keys，點new ssh keys


### 8.Title為自己的命名，下方的key必須到git bash中輸入ssh-keygen --> 按enter --> y --> 按enter，如果不是自己的電腦或是是教室的電腦必須要設定一下密碼，是自己的就按enter-->再次輸入 ，輸入指令-->cat，接著把pub的檔案複製並貼上 -->並把產生的碼全部複製，並貼在第7點中的ssh key的下方，確認無誤就點選Add SSH Key



### 9.到自己的github專案上去點選Code(綠色)，複製SSH下面的網址，到git bash的環境中輸入指令git clone後面再貼上，按enter-->沒有密碼就不需要打，並下載結束




