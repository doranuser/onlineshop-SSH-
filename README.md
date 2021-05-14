# onlineshop-SSH-
<h1>專案說明</h1>
<br>
由於前一個工作擔任美編企劃 主要 負責產品拍攝，做文案、圖像的呈現。<br>

因此希望為能結合前一個工作的作品展現，因此選擇以網路購物網的方式製作。<br><br>


--前端技術--<br>
bootstrap、html、css、javascript、jsp<br><br>

--後段端技術--<br>
java、Spring、Spring MVC、hibernate<br><br>

--資料庫連接--<br>
SQL server資料庫<br>
對應的table有用foreign key跟pk做關連起來<br><br>

table 設計如下<br>
cart<br>
porder<br>
porder_detile<br>
porder_detile_log<br>
customer<br>
products<br>
picture<br><br>

架構設計<br>
1.會員管理<br>
2.購物車<br>
3.訂單系統<br><br>

架構說明<br>
1.產品分為四類，咖啡壺、濾杯、磨豆機、細口壺<br><br>

2.流程<br>
a. 進入login 可以進行登入，如果查無username 則會跳去註冊頁<br>
b. 登入後會記錄Browser的cooki id，判別是否已經登入<br>
c. 選購商品加入購物車，進入購物車前會先做login filter，判別是否已經登入<br>
    <會寫入cart table ，如此一來下次登入時，同個user 購物車內容會保留><br>
d. 購物車確認後，填寫收件者資料及付款方式、收貨方式等<br>
e. 顯示購物的資訊，點選列印按鈕，列印該頁面<br>

3. 針對porder_detile table有做trigger，一旦新增、修改、刪除都會被寫入porder_detile_log table 中<br><br>

頁面呈現如下<br><br>


<img src="https://doranuser.github.io/onlineshop-SSH-/01.JPG" alt="" width="600px"><br><br>
<img src="https://doranuser.github.io/onlineshop-SSH-/02.JPG" alt="" width="600px">

