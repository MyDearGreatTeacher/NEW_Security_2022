# MyFirstSecurityOnline
- 全力啟動你深層的資安戰鬥力！
```
照過來

來點 special 師 輩 秀

兩小時的課程
```
                           
## 課程目標：本課程引領學生透過CTF解題來學習資訊安全的觀念與技術。
## 課程介紹：
```
本次課程從基礎教起，只要你會電腦及強烈的學習態度即可！
我們規劃了趣味性CTF(Capture The Flag)搶旗大賽題目，
讓學生充滿自信的學、快樂的學，
充分享受一個Happy Hacking Day！！
```
## 課程內容：
- 1_透過參與CTF搶旗大賽學習資安實務	
  - CTF搶旗大賽
  - 註冊與登入CTF
  - 起手式---word隱寫術
  - 台灣舉辦的世界級搶旗大賽Hitcon CTF
- 2_網站安全測試	透過簡單的網站安全解題讓學員啟動網站安全測試的興趣
  - 隱藏在註解裡的FLAG
  - Robot.txt的奧秘
  - URL redirection的破招
  - HTML method的奧義
- 3_ 編碼與解碼	你能破解底下的編碼嗎?
  - ASCII   | BASE64  | Base 32  |MORSE code  |DNA編碼
- 4_古典密碼與破密分析	
  - 讓我們檢驗古老時代的密碼技術吧?
    - ROT 13   
    - 凱薩密碼   
    - 密碼棒   
    - Vigenère cipher
  - 也順便體驗 【暴力破解法】與【頻率分析法】的技術


# 1.透過參與CTF搶旗大賽學習資安實務	[YOUYUBE錄影]()

## CTF(Capture The Flag)搶旗大賽
- [令人感動一定要看的影片HITCON in DEFCON 22 CTF Final 紀錄片](https://www.youtube.com/watch?v=XcneHvq1hbY)
  - 你可以看到許多`台灣好厲駭`導師的年輕身影 
- [一次看懂CTF資安攻防賽](https://www.ithome.com.tw/news/102969) 
  - 三大主要CTF資安攻防賽類型
    - 1_解謎式（Jeopardy） 本次教學使用的類型
    - 2_攻防模式（Attack and Defense）
    - 3_King of The Hill(類似搶灘遊戲)
- [ddaa (0xddaa)寫的CTF 的三十道陰影 系列](https://ithelp.ithome.com.tw/users/20121059/ironman/2810)

## 註冊與登入CTF

- 登入CTF平台(上課使用的平台)
- 註冊(register) ==> 點選右上角register按鈕

![註冊](註冊.png)

## 起手式---word隱寫術[YOUYUBE錄影]()

## 台灣舉辦的世界級搶旗大賽Hitcon CTF[YOUYUBE錄影]()

- [HITCON YOUTUBE頻道的影片](https://www.youtube.com/c/HacksInTaiwan/videos)
- [讓我們來解一題Hitcon CTF吧](https://ctf2017.hitcon.org/)  

## 更多台灣舉辦的ctf(以字母順序陳列+請上網搜尋)  若有遺漏煩請告知! 謝謝
- AIS3 CTF
- [AIS3 EOF CTF](https://ais3.org/eof)
- [Balsn CTF](https://balsn.tw/)
- BambooFox CTF
- [MyFirstCTF](https://ais3.org/mfctf/)

## 更多國外cctf資訊==> [CTFtime](https://ctftime.org/)

# 2_網站安全測試 [YOUYUBE錄影](https://youtu.be/n9S-th78_9E)
- 透過簡單的網站安全解題讓學員啟動網站安全測試的興趣

## Web101解題
## Web-1:source code 隱藏在註解裡的FLAG
## web-2: Easy_Robots.txt == >Robot.txt的奧秘
- [Robots.txt - 維基百科](https://zh.wikipedia.org/zh-tw/Robots.txt)
- robots.txt是一種文字檔案，它告訴網路搜尋引擎此網站中的哪些內容是不應被搜尋引擎的搜尋到的，哪些是可以被搜尋引擎搜尋到的。
- robots.txt放在網站伺服器的哪個位置?

## web-3:Robots.txt [學完課程3_編碼與解碼後再來解這題]
- 仔細看提示HINT
- 本題任務是請你找到robots.txt並因此找到flag。
- 提示1 : robots.txt的存放放置
- 提示2 : 相關hex to string及base64 編碼


# 底下兩題是規劃讓學生熟悉curl工具
- [官方網址](https://curl.se/)
- [官方提供的書 Everything curl ](https://curl.se/book.html)
- curl的windows版
  - windows 10以上已經支援
  - [其他版本則需到官方網址下載](https://curl.se/download.html)


![curl.png](curl.png)

- [使用 Curl 來進行發送 HTTP Request封包](https://blog.techbridge.cc/2019/02/01/linux-curl-command-tutorial/)

| 參數 | | 說明 |
| -- | -- | --|
|-X |--request  | 可以加的參數GET,POST,PUT,DELETE,PATCH:使用指定的 http method 來發出 http request| 
| -H | --header    |                        設定 request 裡所攜帶的 header| 
| -i| --include   |                        在 output 顯示 response 的 header| 
| -d| --data       |                       攜帶 HTTP POST Data | 
| -v| --verbose     |                      輸出更多的訊息方便 debug| 
| -u| --user       |                       攜帶使用者帳號、密碼| 
| -b| --cookie      |                      攜帶 cookie（可以是參數或是檔案位置）| 


## web-4:Curl-1 ==> url redirection的破招 [解答影片]()

## web-5:HTTP method ==>HTML method的奧義[解答影片]()

```
curl -X GET -v http://ip:3001/index.php

curl -v http://ip:3001/index.php

curl -X POST -v http://ip:3001/index.php

curl -X OPTIONS  -v http://ip:3001/index.php

curl -X GETFLAG  -v http://ip:3001/index.php
```


## 網站伺服器(web server)與網站應用程式(Web application)


# 3_編碼與解碼 你能破解底下的編碼嗎? [YOUYUBE錄影](https://youtu.be/KVLaB4h5GZU)
- code
- coding
- `en`code
- `de`code
- decoder

# 編碼(encoding)與解碼(decoding) 
- 在計算機的世界有許多 編碼(encoding)與解碼(decoding) 的機制與應用
- [字元編碼(Character encoding)](https://en.wikipedia.org/wiki/Character_encoding):本次課程學習主題
  - 文字(英文字母 vs 世界各國文字)與數字(0,1,....,9)如何被表示成電腦可以處理的0|1
  - [ASCII(American Standard Code for Information Interchange)](https://en.wikipedia.org/wiki/ASCII)
  - BASE64 編碼
  - BASE32 編碼
  - Morse Code 摩斯電碼
  - [Unicode(留給你做報告)](https://en.wikipedia.org/wiki/Unicode)  以`編碼102:第一堂Unicode`當作練習
- telecommunication 有許多 ==> see 網路概論 
  - [曼徹斯特編碼（Manchester coding）](https://en.wikipedia.org/wiki/Manchester_code)
  - [Differential Manchester encoding](https://en.wikipedia.org/wiki/Differential_Manchester_encoding)
    - [Lec-7: Manchester encoding and differential manchester encoding in hindi | Computer Network](https://www.youtube.com/watch?v=3IaB2a8tXLA)
- [HTML URL Encoding](https://www.w3schools.com/tags/ref_urlencode.asp)
- 不勝枚舉.....



## ASCII 編碼與解碼
- [ASCII(American Standard Code for Information Interchange)](https://en.wikipedia.org/wiki/ASCII)
- [ASCII decoder 解碼線上工具](https://www.dcode.fr/ascii-code)

## BASE64 編碼與解碼
- [WIKI 說明](https://zh.wikipedia.org/wiki/Base64)
- [錄影教學](https://youtu.be/pIYU3qnn9bU)

## [Base 32 編碼與解碼](https://en.wikipedia.org/wiki/Base32)
- 留給你當作作業

## MORSE code(摩斯電碼) 編碼與解碼
- [中文版WIKI 說明](https://zh.wikipedia.org/wiki/%E6%91%A9%E5%B0%94%E6%96%AF%E7%94%B5%E7%A0%81)
- [有趣的影片HOW IT WORKS: Morse Code](https://www.youtube.com/watch?v=xsDk5_bktFo)


# 4_古典密碼與破密分析 ==>  Crypto101

- [Classical cipher古典密碼](https://en.wikipedia.org/wiki/Classical_cipher)
- [Classical cipher古典密碼:中文WIKI](https://zh.wikipedia.org/wiki/%E5%8F%A4%E5%85%B8%E5%AF%86%E7%A2%BC)
- 古典密碼兩大類型
  - [替換式密碼substitution cipher](https://zh.wikipedia.org/wiki/%E6%9B%BF%E6%8D%A2%E5%BC%8F%E5%AF%86%E7%A0%81)
    - 凱撒密碼Caesar cipher
    - 維吉尼亞密碼Vigenère cipher
  - 移位式密碼Transposition ciphers
    - 密碼棒scytale 

## 凱薩密碼Caesar_cipher  <== ROT 13 [YOUYUBE錄影](https://youtu.be/tOjZRg20NPQ)
- [凱撒密碼:維基百科說明](https://en.wikipedia.org/wiki/Caesar_cipher)
- [凱撒密碼:中文維基百科說明](https://zh.wikipedia.org/wiki/凱撒密碼)

- 線上解題工具
  - https://planetcalc.com/1434/
  - http://md5decrypt.net/en/Caesar/
  - https://www.xarg.org/tools/caesar-cipher/

-【窮舉法|暴力破解法】:把各種可能的答案都算出來
- 示範解題:Crypto101:ABCTF 2016 : ceasar-salad-10
- 練習題:Crypto101:angstromCTF 2017:The Beginning
- 練習題:Crypto101:RC3 CTF 2016 : salad-100(解不出來,不必緊張)

## 密碼棒 Scytale [YOUYUBE錄影](https://youtu.be/8XbZSa-1GkE)
- [英文WIKI說明](https://en.wikipedia.org/wiki/Scytale)
- [中文WIKI的說明](https://zh.m.wikipedia.org/zh-tw/%E5%AF%86%E7%A2%BC%E6%A3%92)
- 示範解題: Crypto101: EKOPARTY CTF 2015: SCYTCRYPTO


## [Vigenère cipher 維吉尼亞密碼](https://en.wikipedia.org/wiki/Vigen%C3%A8re_cipher)
- [YOUYUBE錄影]
```
plaintext():attackatdawn
keyword "LEMON"
加密後的秘文()為何 ?
```
- [解答Vigenere CIpher](https://www.youtube.com/watch?v=SkJcmCaHqS0)

![Vigenère_square.png](Vigenère_square.png)

## 古典密碼的破密 ==> 【頻率分析法frequency analysis】
- [YOUYUBE錄影]()
- [替換式密碼Substitution cipherの頻率分析法](https://zh.wikipedia.org/wiki/%E9%A2%91%E7%8E%87%E5%88%86%E6%9E%90)
- 解題:使用線上工具http://quipqiup.com/
- 示範解題: Crypto101: Pico CTF 2014 : Substitution
- 題目附件:encrypted.txt
```
tep yhteszxdytxsj rsbp xo yuesgpjpuuszgb

x ryj oesu fsh tep uszgb
oexjxjk oexccpzxjk ongpjbxb
tpgg cp nzxjrpoo jsu uepj bxb
fsh gyot gpt fshz epyzt bprxbp

x ryj snpj fshz pfpo
tyap fsh usjbpz qf usjbpz
slpz oxbpuyfo yjb hjbpz
sj y cykxr ryznpt zxbp

y uesgp jpu uszgb
y jpu iyjtyotxr nsxjt si lxpu
js sjp ts tpgg ho js
sz uepzp ts ks
sz oyf upzp sjgf bzpycxjk

y uesgp jpu uszgb
y byddgxjk ngyrp x jplpz ajpu
qht jsu izsc uyf hn epzp
xto rzfotyg rgpyz
teyt jsu xc xj y uesgp jpu uszgb uxte fsh

hjqpgxplyqgp oxketo
xjbporzxqyqgp ippgxjk
osyzxjk thcqgxjk izppueppgxjk
tezshke yj pjbgpoo bxycsjb oaf

y uesgp jpu uszgb
bsjt fsh byzp rgsop fshz pfpo
y ehjbzpb teshoyjb texjko ts opp
esgb fshz qzpyte  xt kpto qpttpz
xc gxap y oesstxjk otyz
xlp rscp os iyz
x ryjt ks qyra ts uepzp x hopb ts qp

y uesgp jpu uszgb
plpzf thzj y ohznzxop
uxte jpu eszxdsjo ts nhzohp
plpzf cscpjt kpto qpttpz
xgg reyop tepc yjfuepzp
tepzpo txcp ts onyzp
gpt cp oeyzp texo uesgp jpu uszgb uxte fsh

y uesgp jpu uszgb

y uesgp jpu uszgb
y jpu iyjtyotxr nsxjt si lxpu
js sjp ts tpgg ho js
sz uepzp ts ks
sz oyf upzp sjgf bzpycxjk
y uesgp jpu uszgb
plpzf thzj y ohznzxop
uxte jpu eszxdsjo ts nhzohp
plpzf cscpjt kpto qpttpz
xgg reyop tepc yjfuepzp
tepzpo txcp ts onyzp
xgg reyop tepc yjfuepzp
tepzpo txcp ts onyzp
gpt cp oeyzp texo uesgp jpu uszgb uxte fsh

y uesgp jpu uszgb
y uesgp jpu uszgb
teyto uepzp upgg qp
teyto uepzp upgg qp
y tezxggxjk reyop
y usjbzsho ngyrp
isz fsh yjb cp
```
