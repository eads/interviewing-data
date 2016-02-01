#如何訪問大筆資料
繁體中文(Traditional Chinese)

英文(English)[原版發佈於NPR Editorial Training](http://training.npr.org/visual/what-to-do-with-a-big-pile-of-data/)

當面對龐大的數據和資料時，以下的小撇步會幫助你搞懂數字的意義，發現新聞點以及找出能訪問這些數據的問題。

如同訪問一般受訪者一樣，這些技巧並不一定能馬上幫你找出新聞的爆點。事實上，這樣的數據分析其實很少能馬上帶出新聞爆點。不過這也是為什麼學會如何快速地訪問資料在處理新聞時很實用的主因。

在繼續閱讀前，這份指南假設你對於試算表表格和函數有基礎的認識。

註：所用的數據庫為[美國芝加哥市現任職員名字，薪水，職稱和部門的資料](https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w)。

##找到數據相關資料
拿到這份數據後，你的首要工作為找出這份數據所有的相關資料。點擊該[數據網頁](https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w)上的“相關(about)”按紐後，你會看到下列資訊：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/AEF2C647-9219-2EE1-2246-02EC917EAD4D11.jpg)

當你使用這份資料，發表任何東西前，你必須先詳細求證這數據內的資訊。

基於這份數據的發表時間和內容敘述（每季更新），這份數據最新的更新為2014年第四季(Q4, 2014)。不過這只是我們的假設。在使用這份資料前，你還是必須先聯絡這份數據的擁有者藉以求證資料的內容。至少我們知道這份數據是由人資部（Human Resources）公布的，而數據的聯絡人為Eric Phillips。

當你在研究這份數據時，你可以問下列的問題：
- 是誰創造這份數據的？
- 誰負責維護這份數據？
- 數據包含的時間點或時間範圍是什麼時候？
- 數據是如何搜集的？
- 每個欄位是如何整理與算出來的？

##將數據導入試算表中
我們將使用免費且具同時合作功能的Google試算表，若不想用Google試算表的話，Excel也是一個不錯的選擇。

若你手上的數據相當敏感，譬如說與NSA包商前僱員「深喉嚨」史諾登（Edward Snowden)有關的數據，那你大概不會想要把數據放在Google 試算表上，因為Google試算表有機會被政府或駭客駭入。

##整理和格式化你的數據
格式化你的表格會幫助你很多。

調整表格的寬度，你才能完整看到表格內的文字和數字。用數字格式化來讓大數字中間加上逗號，小數加上小數點。貨幣格式則是用在金錢數字上，百分比則是用在分數上。

![alt text](http://training.npr.org/wp-content/uploads/2015/05/13TqCYSHna6cCfw2XT2gTwyDrqygKZbVAjUYOYg11.gif)

按住第一欄欄位名稱下方邊界往下拖曳，這樣就可以鎖定第一行欄位，讓你能剛方便地查看下方的資料。

![alt text](http://training.npr.org/wp-content/uploads/2015/05/1OQadwCZ6y-Xf9rFH0W_HaBmdd_rsjjci4BTEKQ11.gif)

##這樣排序，那樣排序
如果你的數據包含數字的話（例如職員薪水），你可以使用排序功能，一眼就能看出最大數字以及最小數字。要使用排序功能，將滑鼠移至欄位第一欄，點欄位內的倒三角形，然後選擇兩種排序法的其中一種。

兩種排序法的名稱容易讓人誤解。“A → Z” 排序許的意思就是將數據從小排到大，而 “Z → A”則是將數據從大排到小。

我們先把薪水數據庫的數據從大排到小 (“Z → A”)：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1zTnEdLQIHOxrv_ThViVW_2XGUGr6K46i1YHNSA.11.gif)

結果大概就跟猜得差不多，高階公務員像高階警政管理人員和市長的薪水都很高。

接下來我們試著從小到大排序(“A → Z”)：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1ZLITr5M7pDlByLDozoTkPkFzqeDRlQMSrhtZfg11.gif)

阿哈！結果我們發現市長辦公室裡竟然有一個人年薪僅0.96美金。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_053DFABB-EF83-BF23-CDF5-4D8B492BED3011.jpg)
我們快速的[Google一下Steven Koch](https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=steve%20koch%20chicago)，馬上發現他並不只是一名行政秘書，他更是[芝加哥的副市長](http://www.cityofchicago.org/city/en/depts/mayor/press_room/press_releases/2012/august_2012/steve_koch_nameddeputymayorofthecityofchicago.html)，也曾經是華爾街的銀行家，被認為是[芝加哥最有影響力的人之一](http://www.chicagomag.com/Chicago-Magazine/March-2013/Steve-Koch/)。

兩個簡單的排序，就給了我們第一個新聞點。小撇步：目前似乎還沒有人做過這個年薪0.96美金卻具有極大影響力的人的新聞。恩….….

##用樞紐分析表（pivot tables）來組合和計算
樞紐分析表的作用在於數據重組，讓你發現數據標準結構之外意想不到的細節。更確切地說，樞紐分析表能基於數據的分類來做總數計算，求總和以及一般計算。

樞紐分析表常因為複雜又難以理解而令人詬病。不過你如果你先想好你想訪問數據的問題，會讓理解的過程容易些。每個部門有多少員工？每個部門發放的薪資總量是多少？每個部門的薪資中位數是多少？

如果你的問題類似於“每個<種類>中<變數的概況>？”你或許就能在樞紐分析表中找到解答。

讓我們現在開始吧！選擇“數據”選單中的樞紐分析表，然後在“行”中加上你的“分類”。在這個案例中，我們的分類就是“部門”：

首先：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_724D4B2A-42F9-E685-83C6-1BE1DA3ECF5411.jpg)

其次：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_8EF99CD8-CD56-8826-793C-95A8C662AC5211.jpg)

現在，我們就能用“COUNTA”函数計算出每個部門的員工人数：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_13253154-4FE5-8670-F8C9-69DA57370C2211.jpg)

為什麼選擇用“COUNTA”函数呢？其實這只是方法之一，根據先前的經驗和[搜尋](https://support.google.com/docs/answer/3093991?hl=en)，我們知道它的作用是計算數量，計算某個值的數量。當然，分析數據的方法並非只有一種，這就是重要的實驗階段。

你可以隨意嘗試，算出不同的數據概況：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_16E9B6EA-7618-B141-D131-57B81073866D11.jpg)

算出來的這些數據概況有助你理解數據的規模和結構。

在這個案例中，我們可以看到，芝加哥警局僅在員工薪資中就支出了10億美金，比列位第二的資加哥消防局整整高出一倍。

我們還能看到，DoIT（技術創新局，你最好上網查證一下，確定你的訊息）員工的薪資中位數值則是最高的。這可能就是另一個新聞點，或者能為你的新聞提供一定輔助訊息。

##將樞紐分析表複製到新的工作表中
樞紐分析表是一個很有用的工具，但用它來做數據分類和數據分析有時候也是滿麻煩的。用樞紐分析表來做數據的排序有時候會讓你樞紐分析表跑起來很慢或怪怪的，為了防止這種現象，你可以將樞紐分析表的內容複制貼到另一個計算表中。貼上時，記得要選擇”只貼上數字“，否則只是複製貼上了另一份超慢的樞紐分析表。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1gLe3USTH2jCtP9PRawtAAK0AqHPSjOY3tr4ZMQ11.gif)

##將數字以百分比的方式呈現
警察局和消防局支出的總薪資異常龐大，但是這個數字在整體的比例到底佔多少呢？將樞紐分析表複製貼上到新的表格後，你就能用基本的程式進行計算，從中看出端倪。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/ezgif-242909479811.gif)

現在，你就能進行數據整理，統一數據格式，計算各項總數，藉以洞悉數據概況：
![alt text](http://training.npr.org/wp-content/uploads/2015/10/t_D60F3D95-CFF2-018B-D4F7-F85EDFDBA6D211.jpg)

基于數據概况，你能得出這樣的結論，“消防局的薪資支出为4.23億美元，佔城市整體薪資總額的17%。”

做進一步調查後，我們能把薪資支出放在政府總體預算裡來考量，[芝加哥2014年的政府預算為70億美元](http://articles.chicagotribune.com/2013-11-26/news/chi-aldermen-expected-to-ok-emanuels-7-billion-budget-20131126_1_speed-cameras-city-spending-cigarette-tax-increase)，24.3億美元除以70億美元等於0.347。因此，薪資支出占城市總體預算的35％。

作者[David Eads](https://twitter.com/eads)，為新聞應用程式工程師，任職於美國公共廣播電台（NPR）視覺部門。

翻譯林辰峰[Jeremy C.F. Lin](https://twitter.com/Jeremy_CF_Lin)
