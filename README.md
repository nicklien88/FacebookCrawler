這是用來從Facebook(臉書)收集資料的爬蟲程式
=====

原理
###
    
    利用Selenium 套件模擬人類操作瀏覽器，自動登入帳號密碼，自動滾輪網頁下滑，自動點擊網頁上的按鈕，
    再用BeautifulSoup套件取得網頁原始碼，藉由HTML中的標籤、屬性找到要擷取的資料
    tkinter套件設計GUI 圖形介面, 以方便使用者操作
 
    此程式適合用來爬取Facebook 中的個人主頁、紛絲專業、社團的貼文或留言

圖形介面功能說明
###
    帳號: 輸入Facebook的使用者帳號
    密碼: 輸入Facebook的使用者密碼(密碼會以星號顯示)
    網址: 輸入欲爬取的Facebook頁面的網址，頁面需為個人主頁、粉專首頁、社團首頁

搜尋條件
####
    姓名: 輸入某用戶的ID名稱，搜尋特定用戶的貼文或留言。若未輸入，代表搜尋所有貼文或留言
    日期: 輸入日期區間 格式: yyyy-mm-dd，搜尋特定時間內的貼文，若是尋找留言，則代表特定時間內的貼文中的留言
    按讚數: 輸入數字，搜尋大於按讚數的貼文，無法用於留言
    檔名: 輸入檔名，爬取的資料會存成JSON檔, 格式: 檔名.json

按鈕
####
    尋找貼文: 尋找符合條件的貼文
    尋找留言: 尋找符合條件的留言


    可輸入以下範例試試看程式喔

範例測試
####

1. Bos巴菲特線上學院 粉專網址

網址: https://www.facebook.com/buffettonlineschool/<br>
日期: 2020-04-10 2020-04-15<br>
按讚數: 按讚數: 100<br>
檔名: Bos巴菲特線上學院.json<br>
尋找貼文<br>

2. Bos巴菲特線上學院 粉專網址

網址: https://www.facebook.com/buffettonlineschool/<br>
日期: 2020-04-10 2020-04-15<br>
按讚數: 100<br>
檔名: comments in Bos巴菲特線上學院.json<br>
尋找留言<br>
