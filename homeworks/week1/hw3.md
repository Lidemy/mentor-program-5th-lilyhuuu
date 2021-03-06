## [Week 1 hw3] Command line 求生指南


### 有請 Command line 下凡

身為一個數位時代的子民  
每台電腦都會有很多圖示，可以點來點去、複製刪除  
也幾乎每個檔案都有配圖，就算你不會念檔名，  
還是能看圖示認出這是 chrome、那是 word  
這種使用游標、有很多圖形，讓你可以看圖做事的使用畫面，  
就叫做「圖形使用者介面 Graphical User Interface」，簡稱 GUI


但，假如今天好死不死你的滑鼠突然壞了  
你又很想把桌面上某個神秘的檔案盡快刪除  
該怎麼辦呢？如果你會 Command line ，這時候就有解了！  


### 什麼是 Command line？

想像一下，在 50、60 年前  
當時的電腦還是超巨大的奇行種  
也還沒有發明滑鼠這個好東西  
大家在公司必須帶著自己的螢幕和鍵盤  
共用一台超大主機，才能對電腦下指令  
讓電腦幫人腦完成複雜的計算工作  

既然只能用鍵盤來跟電腦對話  
就必須要輸入一些特定的文字來直接命令電腦  
這個概念就是我們今天要學的 Command line  
這種操作方式叫做「命令列介面 Command-line Interface」，簡稱 CUI

Command line 很酷，不用靠滑鼠和圖示   
而是利用鍵盤直接輸入指令來跟電腦溝通  
你會看到的，是個像駭客專用的黑畫面  
這個黑畫面有個名字，叫做終端機 Terminal  
Terminal 就是我們要輸入文字來命令電腦的地方  

你可以把 Terminal 想像成是電腦在用的 line  
可以讓電腦收到你傳的訊，而且他也會在這回傳訊息給你  
只是電腦是個很笨的工具人，你必須要說出特定的指令他才看得懂  
所以不能問他 How are you，他看不懂啦  


跟充滿圖形的 GUI 比起來  
CUI 對新手來說看起來就像宇宙黑洞般神秘又危險  
但其實沒這麼可怕  
反正電腦看得懂的文字不多，你打錯了他只會跟你說看不懂  
就再研究看看怎麼讓他看懂就好了  


### 開始跟電腦傳 line 吧！

首先，要學會開啟 Terminal，這樣你跟電腦才能開始聊天

Mac 可以用快捷鍵 cmd+space 打開 spotlight，輸入 terminal  
開啟後，會出現一個黑畫面，還有個一直在閃動的游標  
恭喜你，成功打開 Terminal 了！  


接著，我們來試著輸入 pwd 然後按下 enter，  
你會發現電腦回應了一行文字，可能會像這樣：`$ /Users/lilyhu`  
恭喜你！成功的跟電腦對話了！  
你可能還看不懂這是什麼意思，但沒關係，等等就會解釋  

現在我們來試試輸入 123，然後按下 enter，  
你會發現電腦回傳了一段文字，告訴你他看不懂你在說什麼  
可能會像這樣：`$ command not found: 123`  
同樣恭喜你，成功的收到第一個錯誤訊息了！  

你可能有發現，剛剛在做的，就是使用 command line 來對電腦下指令  
當電腦接收到看得懂的指令，就會回應你執行的結果  

所以，只要學會正確指令碼，你就可以命令他做事  
像是幫你新增一個叫做 123 的檔案、刪除一張桌面上的圖片  
或是重新命名某個資料夾的名稱  
不用滑鼠，只要會用 Command line，電腦就會乖乖的說到做到！  

不過有個前提是，  
必須要讓電腦知道現在要去哪裡，才能幫你在那邊完成工作  
例如，你希望他在桌面上新增一個叫做 wifi 的資料夾  
就要先傳訊跟他說，誒誒現在移動到桌面，  
先讓他移動過去後，你才能再跟他說新增資料夾的指令  
一個口令一個動作，沒按照順序來他就會跟你說看不懂  

---



### Command line 指令介紹與實作

接下來介紹幾個基本且常用的 Command line 指令

1. pwd: 讓電腦回報目前所在位置
2. ls: 列出目前位置的所有檔案
3. cd: 讓電腦移動到目前所在位置的下一層檔案夾中
4. cd . . : 讓電腦移動到目前所在位置的上一層檔案夾中
5. touch: 建立新檔案 
6. rm: 刪除檔案
7. cp: 複製檔案
8. mv: 移動檔案
9. mkdir: 建立新資料夾
10. rm –r: 刪除資料夾




### 溫馨手把手示範時間

說再多不如直接來！狀況題示範：


* 看一下電腦目前在哪裡，請他列出目前位置有哪些檔案

```
$ pwd
$ ls
```

* 讓電腦從現在的位置移動到桌面，刪除一個叫做 123 的檔案

```
$ cd desktop
$ rm 123
```

* 建立一個叫做 wifi 的資料夾，並在裡面建立一個叫 afu.js 的檔案 

```
$ mkdir wifi
$ cd wifi
$ touch afu.js
```
* 看一下 afu.js 裡面有什麼內容

```
$ cat afu.js
```


### 其他操作小技巧

有幾個小撇步學會了還蠻讚的，就列在這邊吧！

1. cd + tab 鍵: 想跳到 cd test，打 t 直接按 tab 鍵即可選取
3. ls -al：可以看到隱藏檔案
4. 如果檔名中有空格，可以用‘’或“”括號起來
5. clear: 可以清空畫面中全部的操作指令
6. cat: 快速看檔案內容
