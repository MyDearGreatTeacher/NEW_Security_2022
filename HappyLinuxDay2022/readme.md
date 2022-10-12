# HappyLinuxDay2022

# agenda
### Z.上課之前記得先完成預先作業
#### Z1.請先下載這些龐大的系統
- HappyLinuxDay會用到的Kali Linux [下載點](https://drive.google.com/file/d/1m620Z7KAOSUOLdFH92FYLE2NINb-vJsn/view?usp=sharing)
- HappyPythonDay會用到的Ubuntu Linux 18.04 LTS(已安裝好pwntools)  [下載點](https://drive.google.com/file/d/1aP-qCFP6jKsGYXtKy9ahwZleQSENEi7C/view?usp=sharing)

#### Z2.下載並安裝virtual box + 匯入你要用的linux
- 在你的電腦下載 [virtual box](https://www.virtualbox.org/wiki/Downloads) 並安裝完成 [Virtualbox安裝:YOUTUBE影片](https://youtu.be/FC0CX71aGnc)
- 匯入你要用的linux  [YOUTUBE影片](https://youtu.be/GTpQR7fZcwE)

#### Z3.後續會使用到的
- 首先請申請Google帳號
- 再請申請 [github帳號](https://github.com/)

### A.快速體驗linux作業系統(上課時數: 1 小時左右課程)
```
1_1_認識Linux作業系統:多人使用與多工作業
    作業系統功能
    linux 核心(kernels)與Shell
    Linux 發行版本(distributions)
    Linux的目錄結構
   
1_2_基本指令
     檔案與目錄操作指令
     使用CTF學linux 指令[講師依照自己選擇題目解題]
     redirection(重定向)與pipe(管道)
```
- 進階練習
  - 使用VirtualBox建置Linux學習系統
  - Kali linux的認識
### B.隱寫術 Steganography快速入門 (上課時數: 1 小時左右課程)

- 1_認識 隱寫術 Steganography 
- 2_圖片隱寫術之1:基本入門技_使用linux 基本指令file|strings|grep
- 3_圖片隱寫術之2:圖片內嵌解答圖片的解題
  - 你必須會回答 檔案格式(file signature)
  - 會使用hex編輯器分析檔案
  - 會使用Linux的dd、binwalk指令解圖片隱寫術
- 4_圖片隱寫術之3:圖片的metadata    

### C.使用Linux進行網路鑑識分析(進階課程 上課時數:2 小時)
- 1.認識wireshark
- 2.網路鑑識分析第一步:使用file 和 string 指令進行分析
- 3.使用wireshark檢視出user使用的瀏覽器版本號
- 4.使用wireshark分析HTTP Basic Authentication(認證)封包







## 進階研讀 可上網
- [Linux 指令大全：工程師活用命令列技巧的常備工具書 (全新升級版) William Shotts 邱世華  博碩文化(2022)](https://www.tenlong.com.tw/products/9786263331075?list_name=srh)


## 作業1:完成底下linux練習
```
https://overthewire.org/wargames/bandit/
```
## 作業2:第二階段學 [ 找書學或上網找資料 ==> 整理到你的GITHUB]
```
linux檔案處理指令  cp rm chmod...
linux檔案壓縮與打包指令 zip tar uzip ...
linux系統管理指令  ps top ...
Linux記憶體臉管理指令 free ...
linux使用者管理指令  useradd userdel passwd
Linux網路指令 wget ssh ...
...

