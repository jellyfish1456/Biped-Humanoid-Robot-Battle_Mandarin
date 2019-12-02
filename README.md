<div align=center><img width="450" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/logo1.jpg"/></div>

雙足機器人是由鈦合金所製作的人型機器人。普遍而言，雙足機器人擁有一個軀幹，一個頭部，兩隻手以及兩條腿。此外，機器人不只需要結合硬體與軟體知識，還需要整合電機、機械、資工等科系的專業知識，而這正是跨領域學習的最佳學習要素。在硬體方面，我們將會學習如何操作、修復各種感測器以及馬達。在軟體方面，我們將會使用Visual-basic like這樣的程式語言。此機器人是從[Robosmart Technology](http://robosmart.com.tw/zh-tw/classes_con.php?id=NDU=)購買的，它提供了建構自己機器人的機會。現在，我們將開始設計一個格鬥機器人，我們可以根據需求自由的設計它。

<div align=center><img width="450" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/3.jpg"/></div>

## 目錄

  * [零件](#零件)
  * [安裝](#安裝)
  * [程式語法](#程式語法)
  * [機器人動作編輯](#機器人動作編輯)
  * [前置作業](#前置作業)
  * [檢查與開始](#檢查與開始)
  * [問題討論](#問題討論)
  * [影片](#影片)
  * [參考程式碼](#參考程式碼)
  * [參考來源](#參考來源)
  * [成員](#成員)
  * [榮譽](#榮譽)
  * [感謝](#感謝)

# 零件

一個雙足機器人主要包含： 
* 機器人
* Innovati Servo Commander 16控制模塊
* IQ4516HV伺服馬達
* CC2541 2.4-GHz藍芽
* USB Mini-B
* ps2無線手把

電池：
* Desire Power V8 11.1V 1300mAh 35C-70C 3S鋰電池
* 平衡充電器



# 安裝

操作系統：Microsoft Windows 10<br/>
安裝 [innoBASIC Workshop 2](http://www.innovati.com.tw/website/down/html/?113.html)以執行代碼。
![pic1](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/1.jpg)


這個操作系統包含了幾個部份：innoBASIC Workshop 是一個安裝在電腦上的軟體平台，提供使用者以innoBASIC程式語言編輯、編譯及下載程式；終端視窗為程式執行時的人機介面和除錯平台；完成的程式碼透過USB，下載到BASIC Commander。BASIC Commander提供三種功能：第一個是通用的I/O；第二個是cmdBUS (TM)，透過它可同時並聯32個利基科技的週邊模組。第三個是DEBUG介面，用來讓innoBASIC Workshop 終端視窗 對BASIC Commander 上傳或下傳資料。
 ![pic25](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/25.jpg)

此操作系統適用於IBM或與其相容的個人電腦，Windows 98或以上的版本/2000/ME/XP/Vista等作業系統均可使用。電腦須有USB 1.1 /2.0 接頭，用來下載程式碼及除錯。

# 程式語法

# 機器人動作編輯

在Windows search裡搜尋並且打開InnoBASIC Workshop 2 commander <div align=center><img width="300" height="500" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/17.jpg"/></div><br/>
 
在命令元裡的是程式碼編輯器
![pic12](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/12.jpg)
 
2. 在上方編輯欄點擊以下的圖示 <div align=center><img width="100" height="100" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/5.jpg"/></div><br/>


3. 它將顯示一個窗口。我們在工具包預設中選擇"Default"，然後在左側使用的模塊中選擇"Servo commander 16"。按"OK"。
![pic27](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/27.jpg)

然後，它會彈出一個警告標誌，警告您檢查伺服馬達的位置。按"OK"。

![pic28](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/28.jpg)

4. 以下是使用Innovation motion editor編輯伺服馬達值的步驟。

 (I) 機器人的動作編成號碼從1到200。

 (II) CH0, CH1, ....到 CH15代表了每一個伺服馬達的編號(當我們勾選各自的ID時，將會使伺服馬達激活，開始運作)。

 (III) 它可以藉由輸入調整數值或是按一下拉桿來調整伺服馬達的角度值。伺服馬達的角度是介於800 到 2200。

 (IV) “時間”代表了當馬達的角度變換時，會在這個我們指定的時間內變換完成，時間單位為毫秒(ms)。
 
 (V) 將此動作編號的馬達角度數據以(.ftxt)儲存至電腦或從電腦讀取(.ftxt)檔案。

 (VI) 將此動作編號的馬達角度數據以(.ftxt)儲存至Innovati Servo Commander 16控制模塊或從Innovati Servo Commander 16控制模塊讀取(.ftxt)檔案。

 ![pic25](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/29.jpg)

5. 在編輯好所有程序後，使用USB Mini-B連接電腦和機器人，並且在InnoBASIC Workshop 2 commander 中點擊"build"以將程序輸入到機器人裡。
<div align=center><img width="100" height="100" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/11.jpg"/></div><br/>

# 前置作業
  
(1) 伺服馬達

下面這張照片是伺服馬達（注意：伺服馬達角度範圍在800~2200）。
<div align=center><img width="300" height="300" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/7.jpg"/></div><br/>

  * 保養:<br/>
      如果伺服馬達運轉不正常 舉例來說：冒煙或卡住 請立即停止馬達運轉 你可以換一個新的馬達或是修理它。
     
  * 位置:<br/>
     機器人總共有15個馬達，下面這張圖是各個馬達在機器人中的編號<br/>
     <div align=center><img width="300" height="300" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/10.jpg"/></div><br/>
     
(2) 電池
下圖為電池(注意:電池電壓範圍為10伏倒12.6伏) 。

<div align=center><img width="400" height="300" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/34.jpg"/></div><br/>
        
 * 充電:<br/>
     將電池連接充電器。
       <div align=center><img width="450" height="350" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/35.jpg"/></div><br/>
       
   以下的步驟為如何使用平衡充電器
   
    1.按"Stop"並選擇"Lipo"。
   
    2.按"+"並選擇balance mode。
   
    3.按"Start"。當電池充飽時，充電器會響起，請按"Stop"。
   <div align=center><img width="450" height="350" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/36.jpg"/></div><br/>  

## 注意

 * 1. 在進行機器人動作編程或使用機器人時，應觀察伺服馬達的溫度是否過高。如果它太高，請停止使用它，否則伺服馬達可能損壞或崩潰。
 * 2. 伺服馬達的角度從800到2200。請小心不要超出這個範圍。
 * 3. 當你發現伺服馬達無法執行操作或異常執行一些奇怪的動作時。請立即停止使用它並嘗試更換新的馬達。
 * 4. 每次使用機器人之前，請確認所有螺釘均已正確鎖緊，以免因零件鬆動而造成損壞。.
   5. 在使用電池之前，請檢查電池電壓。 如果電壓小於10V，請使用平衡電池充電器對其進行充電。電池全滿的電壓為12.60V。
	

# 檢查與開始

請先檢查機器人是否充滿電。

<div align=center><img width="600" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/31.jpg"/></div>

拿起PS2握把並靠近機器人。

<div align=center><img width="450" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/32.jpg"/></div>

將電池與機器人連接。

  <div align=center><img width="600" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/18.jpg"/></div><br/>

在PS2搖桿按下 "START" 按鈕來連接機器人。當機器人成功連接時，機器人會呈現僵直狀態並且伺服馬達會固定住。如果沒有成功連接，PS2搖桿上的紅色的指示燈會不斷地閃爍
 
<div align=center><img width="600" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/33.jpg"/></div>

  
這裡我們使用ps2無線搖桿去控制機器人

![pic24](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/14.jpg)


當機器人成功連接時，機器人會呈現僵直狀態並且伺服馬達會固定住。


注意: 這些按鍵可以自己做更換!



## 討論

1.  * Q:如果機器人沒辦法在不同地面走路保持穩定我們應該怎麼辦？

      A:最近我們有學到如何設計一台在不同環境中都可以適應的機器人 現在我們可以手動的調整機器人。
      
2.  * Q:機器人可以做任何我們想要的動作嗎？

      A:當然可以 你可以設計任何你想要的動作並自行實行你的的想法。
      
3.  * Q:機器人可以應用在哪？

      A:有許多的應用 最近我們完成了機器人體操而且最近跟電腦視覺一起應用。
      
4.   * Q:請問使用的程式語言是什麼?

     * A: Visual basic-like 的程式語言。
     
5.   * Q: 要如何組裝機器人?

     * A: 請參照網站以及按照步驟組裝。
     
如果您有任何問題, 請告知我們:

haha871116@gmail.com

jason3067812@gmail.com

leo32448@gmail.com     

## 影片

體操

[單手倒立](https://www.youtube.com/watch?v=5fRVJbHhV6Q)
	   
[跳轉](https://www.youtube.com/watch?v=VnRADacrUuY)
    
[後翻](https://www.youtube.com/watch?v=si86ftxEGCs)


## 參考程式碼

參考程式碼將會於競賽結束後上傳

## 參考來源

https://en.wikipedia.org/wiki/Humanoid_robot

http://robosmart.com.tw/zh-tw/classes_con.php?id=NDU=


## 感謝

我們特別感謝林柏江教授擔任我們的指導教授

我們也感謝在這一路上幫助過我們的同學，老師們
