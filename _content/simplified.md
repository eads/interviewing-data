#如何分析大笔数据
简体中文(Simplified Chinese)

英文(English)[原版发布于NPR Editorial Training](http://training.npr.org/visual/what-to-do-with-a-big-pile-of-data/)

当面对庞大的数据资料时，以下的几条小贴士能帮助你理解数字的意义，发现数据中的新闻点，找出需要追问的后续问题。

如同采访一般受访者一样，这些技巧不一定能帮你立刻找出新闻中的爆点。事实上，通过这样的数据分析并不能让你得出多了不起的洞见。不过，这也正是为什么学会如何迅速地针对数据提出问题十分重要。

这份指南主要针对那些对数据工作表和函数有基础认识的读者。

注：所用的数据库为美国芝加哥[现任职员姓名，薪资，职称和部门数据](https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w)。

##找到与你数据相关的其他资料
拿到数据后，你的首要工作是找出与这份数据相关的的所有资料。点击[该数据网页](https://data.cityofchicago.org/Administration-Finance/Current-Employee-Names-Salaries-and-Position-Title/xzkq-xp2w)上的“相關(about)”上的“关于(about)”按钮后，你会看到以下信息：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/AEF2C647-9219-2EE1-2246-02EC917EAD4D11.jpg)

在你发表任何基于这份数据得出的结论前，你必须首先保证这份数据中的所有细节真实有效。

基于这份数据的发表时间和内容叙述（每季更新），数据最新的更新时间为2014年第四季度(Q4, 2014)。不过这只是一个假设，在使用这份资料前，你还是必须先联络这份数据的拥有者求证资料的内容。至少我们知道这份数据是由人力资源部（Human Resources）公布的，而数据的负责人为Eric Phillips。

当你在研究这份数据时，你可以问以下的一些问题：
- 这份数据的创造者是谁？
- 谁负责维护这份数据？
- 数据的时间点或时间范围是什么时候？
- 数据的搜集方式？
- 每个栏位是如何整理与计算出来的？

##将数据导入工作表中
我们将使用免费的的Google工作表，它的好处在于方便数据共享和团队合作。当然，Excel也是一个不错的选择。

若你手上的数据相当敏感，譬如说与NSA承包商前雇员斯诺登（Edward Snowden)有关的数据，最好还是别把数据上传到Google工作表上，因为它有可能会被政府或骇客入侵。

##整理和格式化你的数据
统一数据的格式会对你之后的工作有很大的益助。

调整表格的宽度，你才能完整看到表格内的文字和数字。用数字格式化在大数字中加上逗号，在小数前加上小数点。货币格式化可以用在金钱数字有关的数据中，百分比则是用在分数上。

![alt text](http://training.npr.org/wp-content/uploads/2015/05/13TqCYSHna6cCfw2XT2gTwyDrqygKZbVAjUYOYg11.gif)

按住第一行字母下方的边界往下拖曳，这样就可以锁定第一行栏位，让你能更方便地浏览下方的资料。

![alt text](http://training.npr.org/wp-content/uploads/2015/05/1OQadwCZ6y-Xf9rFH0W_HaBmdd_rsjjci4BTEKQ11.gif)

##这样排序，那样排序
如果你的数据包含数字的话（例如职员薪资），你可以使用排序功能，方便找出其中的最大数字和最小数字。要使用排序功能，将鼠标移至栏位第一行，点击栏位中的倒三角形，然后选择两种排序法的其中一种。

两种排序法的名称容易让人误解。“A → Z”排序的意思就是将数据从小到大排列，而“Z → A”则是将数据从大到小排列。

我们先把薪水数据库的数据从大排到小(“Z → A”)：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1zTnEdLQIHOxrv_ThViVW_2XGUGr6K46i1YHNSA.11.gif)

结果大概就跟你的猜想八九不离十，高级公务员像公安管理人员和市长的薪水都位列前几名。

接下来我们试着从小到大排序(“A → Z”)：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1ZLITr5M7pDlByLDozoTkPkFzqeDRlQMSrhtZfg11.gif)

阿哈！结果我们发现市长办公室里竟然有一个人年薪仅0.96美金。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_053DFABB-EF83-BF23-CDF5-4D8B492BED3011.jpg)
我们快速的[Google搜索一下Steven Koch](https://www.google.com/webhp?sourceid=chrome-instant&ion=1&espv=2&ie=UTF-8#q=steve%20koch%20chicago)，马上发现他并不只是一名行政秘书，他更是芝加哥的[芝加哥的副市长](http://www.cityofchicago.org/city/en/depts/mayor/press_room/press_releases/2012/august_2012/steve_koch_nameddeputymayorofthecityofchicago.html)，，也曾经是华尔街的银行家，被认为是[芝加哥最有影响力的人之一](http://www.chicagomag.com/Chicago-Magazine/March-2013/Steve-Koch/)。

两个简单的排序，就给了我们第一个新闻点。小贴士：目前似乎还没有人做过这个年薪0.96美金却具有极大影响力的人的新闻。恩….….

##用数据透视表（pivot tables）来组合和计算
数据透视表的作用在于数据重组，让你发现数据标准结构之外意想不到的细节。更确切地说，数据透视表能基于数据的分类进行计数、求和和计算。

透视表的缺点在于它非常复杂，又难于理解。如果你能带着问题来看，也许理解起来更容易一些。每个部门有多少员工？每个部门发放的薪资总量是？每个部门中的工资中值是？

如果你的问题类似于“每个<种类>中的<某种变量的概况>？”你也许就能在数据透视表中找到答案。

让我们现在开始吧！选择“数据”菜单中的数据透视表，然后在“行”中添加你的<分类>。在这个案例中，我们的分类就是“部门”：

首先：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_724D4B2A-42F9-E685-83C6-1BE1DA3ECF5411.jpg)

其次：

![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_8EF99CD8-CD56-8826-793C-95A8C662AC5211.jpg)

现在，我们就能用“COUNTA”函数计算出每个部门的员工人数：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_13253154-4FE5-8670-F8C9-69DA57370C2211.jpg)

为什么选择“COUNTA”函数？其实这只是方法之一，根据经验之前的经验和[搜索](https://support.google.com/docs/answer/3093991?hl=en)，我们知道“COUNTA”函数的作用是计数，计算某个值的数量。当然，分析数据的方法并非只有一种，我们还处在最初的试验阶段。


你可以随意尝试，汇总出不同的数据概况：
![alt text](http://training.npr.org/wp-content/uploads/2015/05/t_16E9B6EA-7618-B141-D131-57B81073866D11.jpg)

概括出的这些数字有助你理解数据的规模的结构。

在这个案例中，我们可以看到，芝加哥警察局仅在员工薪资中就支出了10亿美金，比位列第二的芝加哥消防局整整高出一倍。

我们还能看到，DoIT（技术创新局，你最好上网查一下，确定部门全称是什么）员工的工资中值最高。这可能成为另一个可以做的故事，或者能为你的故事提供一定辅助信息。

##将数据透视表复制到新的工作表中
数据透视表是一个非常有用的工具，但用它来 ​​做数据分类和数据分析的难度也非常大。做数据分类可能会导致你的数据透视表运行起来异常缓慢，为了防止这种现象，你可以将透视表复制粘贴到另一张工作表中去。粘贴时，切记要选择“粘贴值”，否则只是复制了另一张运行缓慢的透视表。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/1gLe3USTH2jCtP9PRawtAAK0AqHPSjOY3tr4ZMQ11.gif)

##将数字以百分比的形式呈现
警察局和消防局支出的總薪資異常龐大，但是這個數字在整體的比例到底佔多少呢？將樞紐分析表複製貼上到新的表格後，你就能用基本的程式進行計算，從中看出端倪。
![alt text](http://training.npr.org/wp-content/uploads/2015/05/ezgif-242909479811.gif)

现在，你就能进行数据整理，统一数据格式，计算各项总量，然后得出你的数据概况：
![alt text](http://training.npr.org/wp-content/uploads/2015/10/t_D60F3D95-CFF2-018B-D4F7-F85EDFDBA6D211.jpg)

基于数据概况，你能得出类似这样的结论，“消防局的薪资支出为4.23亿美元，占城市整体薪资总量的17%。”

做进一步调查后，我们能把薪资支出放在政府总体预算里来考量。[芝加哥2014年的政府预算为70亿美元](http://articles.chicagotribune.com/2013-11-26/news/chi-aldermen-expected-to-ok-emanuels-7-billion-budget-20131126_1_speed-cameras-city-spending-cigarette-tax-increase)，24.3亿美元／70亿美元＝ 0.347。因此，薪资支出占城市总体预算的35％。


作者[David Eads](https://twitter.com/eads)，新闻应用程序员，供职于美国公共广播电台（NPR）视觉部。

翻譯张洁倩[Jieqian Zhang](https://twitter.com/Jieqian_Zhang)
