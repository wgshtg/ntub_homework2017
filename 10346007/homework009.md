1.在 Rails 的 config/routes.rb 檔案中，resources:users 跟 resource :user 有何不同?
使用resources會幫忙做出8條不同的路徑，且對應到Controller的7個方法；
如果使用resource只會產生7條路徑，也就是說，會少一條index的路徑，並且不會路徑不會含有:id。

2.在 Rails Route 的寫法中，member 跟 collection 有何不同? 該在什麼時候使用哪一種?
使用member所產生出的路徑會帶有id，id會傳到Controller裡變成params變數的一部分，collection則沒有id，通常用在多筆資料，member則是用在單筆資料上。
