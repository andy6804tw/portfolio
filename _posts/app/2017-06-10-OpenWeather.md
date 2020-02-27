---
title:  "OpenWeather天氣"
subtitle: ""
author: "APP"
avatar: "img/icon/app.png"
image: "img/app/app-03.png"
date:   2017-06-10
---

Android、Http Request、SQLite、Firebase

## 簡介
我們團隊是一群大學學生，收集了世界各地天氣資訊，並且使用OpenData政府公開資料為依據，以不同的角度去欣賞天氣 ☀☁☂

-以視覺圖像的方式讓您了解現在的天氣概況
-使用GPS偵測目前位置，顯示目前所在地的即時天氣
-目前狀況掌握今日高低溫以及目前體感溫度
-風速風向搭配動畫一目了然
-詳細的氣壓、濕度、能見度資訊
-天文方面顯示日出日落時間，搭配仰角顯示目前太陽所在位置
-提供詳細的氣象資訊，包括五日十日天氣預報
-Android6.0初次執行時會要求GPS的存取權限，允許才能正常執行哦~
-初次執行App會建立資料庫，請確認GPS是否有開啟，若首次執行閃退是正常現象(待解決)，再次開啟App即可正常運作
-App背景圖片正急尋原作者，若看到請與我們聯絡哦 !

公開資料來源:行政院環境保護署、中央氣象局、Yahoo Weather API

## 功能介紹
首次開啟App會要求位置的存取權限，並且會依據當下的GPS經緯度利用Google Map API轉換成地址，擷取到位置訊息再使用Yahoo Weather API去查詢該地的即時天氣狀況，包含目前溫度、風速、風向、大氣、氣壓、天文、以及十日的天氣預報供使用者即時查閱。
為了解決離線瀏覽的問題我們設計了一個資料庫存取這些政府公開資料，並由手機SQLite資料庫去實作，此外您可以使用此App在世界的任何地方，因此我們還特別加入了多國語言功能將介面英文化，還搭配不同的度量衡為使用者做個人化的設定，例如華視與攝氏的選擇。

![](img/app/app-03-1.png)

第二部分環境我們撈取行政院環保署的供該資料作為資料源，包含當地紫外線以及空氣品質AQI與PM2.5，在本App中不僅僅只是視覺畫呈現資訊，且依據當下的即時狀況未使用者做出即時的防護措施免於週遭的有害物質，此外資料撈取的依據我們是使用目前經緯度和環保署所提供的空氣品質監測站基本資料中的每筆測站經緯度利用Haversine formula大圓距離換算求面上兩點最短距離，找出哪筆測站資料與目前所在的位置最近，且提供給使用者資訊。

![](img/app/app-03-2.png)

![](https://github.com/andy6804tw/OpenWeather/raw/master/Screenshot/demo.gif)

#####  因APP尚未繼續維護，暫時下架。

## 2017 嘉義黑蚵松 地方開放資料戰
🥈獲獎名次：嘉義黑蚵松-地方開放資料戰(資料視覺化組)【第二名】

![](img/app/app-03-5.png)
![](img/app/app-03-3.jpg)
![](img/app/app-03-4.jpg)

參加經濟部工業局舉辦的Open Data黑客松競賽，運用政府所提供的公開資料做資料清理與視覺化，並釋放資料集與開源程式碼供民眾存取。
![](img/app/app-03-5.jpg)


GitHub: [Link](https://github.com/andy6804tw/OpenWeather)

重灌狂人報導: [Link](https://briian.com/42979/)

經濟部工業局報導: [Link](https://opendata.tca.org.tw/index.php/article/readfull/4/15)

2017 嘉義黑蚵松 地方開放資料黑客松獲獎作品介紹: [Link](https://opendata.tca.org.tw/index.php/article/readfull/4/22)

#2017嘉義黑蚵松 #資料視覺化組 #第二名
