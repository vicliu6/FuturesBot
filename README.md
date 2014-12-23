FuturesBot - 台指期當沖自動交易機器人
===========
作者：[Philipz](mailto:philipzheng@gmail.com)、[Blog](http://blog.everfine.com.tw/)

網站：[TradingBot 開放原始碼程式交易系統](http://www.tradingbot.com.tw/)、[Facebook粉絲團](http://www.facebook.com/tradingbot)

軟體授權：Apache License, Version 2.0，請見license.txt

1. 使用環境建置

    1. 安裝 [Java Runtime Environment](https://java.com/zh_TW/download/manual_java7.jsp)
    2. 安裝 [NodeJS](http://nodejs.org/download/)
    3. 安裝接收報價必要 library
    ```
    npm install net mqtt
    ```
    
2. 使用方法 - 修改程式包裝成 Jar 檔

    1. 安裝 [Ant build](http://ant.apache.org/)
    2. 到 FuturesBot 目錄執行 ant ，就會產生好 newfutures.jar
    3. 複製 newfutures.jar 到 VM 虛擬機上的 C:\ ，就完成程式改版佈署。

3. 下單機

    1. 建議使用下單大師，[http://moneyprinter.pixnet.net/blog](http://moneyprinter.pixnet.net/blog)
    2. 或者，請參閱[程式交易經驗分享系列(4) - 下單機設定及系列回顧](https://blog.everfine.com.tw/4/)

4. 程式簡易說明

    1. 主要接受TCP Socket程式為SocketServer.java
    2. 策略邏輯為NewDdeClient.java
    3. 目前設定需配合Dropbox使用，亦可自行修改不使用
    4. GetWednesday.java是檢查每個月台指期和摩台期結算日
    5. 請自行設定排程時間，於每日早上八點四十五分之前執行

### 不想自行建置執行環境可直接下載 VM 虛擬機映像檔

歡迎大家加入討論程式交易，[TradingBot 粉絲團](http://www.facebook.com/tradingbot)或是[Coco-in討論區 - TradingBot程式交易機器人](http://www.coco-in.net/forum-140-1.html)

若需要支援服務，還請小額贊助，支持永續發展此TradingBot。感謝！
聯絡資訊：[service@tradingbot.com.tw](service@tradingbot.com.tw)
