# Biped-Humanoid-Robot-Battle_Mandarin(中文版)

雙足機器人是由鈦合金所製作的人型機器人。普遍而言，雙足機器人擁有一個軀幹，一個頭部，兩隻手以及兩條腿。此外，機器人不只需要結合硬體與軟體知識，還需要整合電機、機械、資工等科系的專業知識，而這正是跨領域學習的最佳學習要素。在硬體方面，我們將會學習如何操作、修復各種感測器以及馬達。在軟體方面，我們將會使用Visual-basic like這樣的程式語言。此機器人是從[Robosmart Technology](http://robosmart.com.tw/zh-tw/classes_con.php?id=NDU=)購買的，它提供了建構自己機器人的機會。現在，我們將開始設計一個格鬥機器人，我們可以根據需求自由的設計它

<div align=center><img width="450" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/3.jpg"/></div>

## 目錄

  * [零件](#零件)
  * [安裝](#安裝)
  * [調整](#調整)
  * [伺服馬達](#伺服馬達)
  * [開始](#開始)
  * [問題討論](#問題討論)
  * [影片](#影片)
  * [參考程式碼](#參考程式碼)
  * [參考來源](#參考來源)
  * [感謝](#感謝)

## 零件

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



## 安裝

操作系統：Microsoft Windows 10<br/>
安裝 [innoBASIC Workshop 2](http://www.innovati.com.tw/website/down/html/?113.html)以執行代碼
![pic1](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/1.jpg)

## 調整




在Windows search裡搜尋並且打開InnoBASIC Workshop 2 commander <div align=center><img width="300" height="500" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/17.jpg"/></div><br/>
 
Inside the commander is the code editor.
![pic12](https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/12.jpg)
 
在上方編輯欄點擊以下的圖示 <div align=center><img width="100" height="100" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/5.jpg"/></div><br/>

他不只可以通過調整數值來改變馬達的轉動角度，還可以改變馬達的時間以及速度。<br/>
CH0, CH1, ....to CH15代表各個獨立的馬達。<br/>

在頁面底部，左側使我們能夠在此電腦上做保存以及加載文件;右側則是讓我們能將文件保存以及加載到機器人的cmu中。
<div align=center><img width="700" height="500" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/4.jpg"/></div><br/>

在編輯好所有程序後，使用USB Mini-B連接電腦和機器人，並且在InnoBASIC Workshop 2 commander 中點擊"build"以將程序輸入到機器人裡。
<div align=center><img width="100" height="100" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/11.jpg"/></div><br/>



## 伺服馬達

下面這張照片是伺服馬達（注意：伺服馬達角度範圍在800~2200）
<div align=center><img width="300" height="300" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/7.jpg"/></div><br/>

  * 保養：<br/>
      如果伺服馬達運轉不正常 舉例來說：冒煙或卡住 請立即停止馬達運轉 你可以換一個新的馬達或是修理它
  
  * 位置：<br/>
      機器人總共有15個馬達，下面這張圖是各個馬達在機器人中的編號<br/>
     <div align=center><img width="300" height="300" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/10.jpg"/></div><br/>
  
  
## 開始

* 首先，我們要確認控制器和電池的電量是否完全充滿
* 第二步，將電池連接機器人
* 第三步，觀察控制器是否成功連接到機器人（紅色指示燈)

<div align=center><img width="600" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/18.jpg"/></div><br/>

  這裡我們使用ps2無線搖桿去控制機器人
  
  <div align=center><img width="450" height="450" src="https://github.com/christw16/Biped-Humanoid-Robot-Battle/blob/master/img/14.jpg"/></div>

  我們按下無線搖桿上的START按鈕。如果以連接上機器人，機器人會呈現僵直狀態，馬達會固定住。
  
  如果未連接上機器人，搖桿上的紅色只是燈會一直呈現閃爍狀態。
  
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


## 感謝

我們特別感謝林柏江教授擔任我們的指導教授

我們也感謝在這一路上幫助過我們的同學，老師們
