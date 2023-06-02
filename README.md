
#### 为中文自然语言处理领域发展贡献语料

<a href='https://www.SuperCLUEAI.com'>中文通用大模型匿名对战评价基准，SuperCLUE琅琊榜</a>

<a href="https://github.com/CLUEbenchmark/SuperCLUE">SuperCLUE: 中文通用大模型综合性测评基准</a>


*** update ****

中文任务基准测评，10大任务 & 9个模型一键运行、详细测评：

Language Understanding Evaluation benchmark for Chinese(<a href='https://www.CLUEbenchmarks.com'>CLUE benchmark<a/>): run 10 tasks & 9 baselines with one line of code, performance comparision with details.
    
Releasing Pre-trained Model of <a href="https://github.com/brightmart/albert_zh">ALBERT_Chinese</a>:

Training with 30G+ Raw Chinese Corpus, xxlarge, small version and more, Target to match State of the Art performance in Chinese with 30% less parameters, 2019-Oct-7, During the National Day of China!</a>

语料库将会不断扩充。。。

一期目标：10个百万级中文语料 & 3个千万级中文语料(2019年5月1号)

二期目标：30个百万级中文语料 & 10个千万级中文语料 & 1个亿级中文语料（2019年12月31日）

Update： 增加高质量社区问答json版(webtext2019zh)，可用于训练超大规模NLP模型；添加520万翻译语料(translation2019zh)。


#### 1.维基百科(wiki2019zh)，100万个结构良好的中文词条
#### 2.新闻语料(news2016zh)，250万篇新闻，含关键词、描述
#### 3.百科问答(baike2018qa)，150万个带问题类型的问答
#### 4.社区问答json版(webtext2019zh)，410万个高质量社区问答，适合训练超大模型
#### 5.翻译语料(translation2019zh)，520万个中英文句子对

#### 为什么需要这个项目

中文的信息无处不在，但如果想要获得大量的中文语料，却是不太容易，有时甚至非常困难。在2019年初这个时点上，

普通的从业者、研究人员或学生，并没有一个比较好的渠道获得极大量的中文语料。笔者想要训练一个中文的词向量，

在百度和github上上搜索了好久，收获却很少：要么语料的量级太小，要么数据过于成旧，或需要的处理太复杂。

不知道你是否也遇到了这样的问题？

我们这个项目，就是为了解决这一问题贡献微薄之力。


1.维基百科json版(wiki2019zh)
-------------------------------------------------------------------------

#### 104万个词条(1,043,224条; 原始文件大小1.6G，压缩文件519M；数据更新时间：2019.2.7)
<a href='https://drive.google.com/file/d/1EdHUZIDpgcBoSqbjlfNKJ3b1t0XIUjbt/view?usp=sharing'>Google Drive下载</a> <a href='https://pan.baidu.com/s/1uPMlIY3vhusdnhAge318TA'> 或 百度云盘</a> 


#### 可能的用途：

    可以做为通用中文语料，做预训练的语料或构建词向量，也可以用于构建知识问答。

#### 结构：

 
    {"id":<id>,"url":<url>,"title":<title>,"text":<text>} 其中，title是词条的标题，text是正文；通过"\n\n"换行。

#### 例子：

    {"id": "53", "url": "https://zh.wikipedia.org/wiki?curid=53", "title": "经济学", "text": "经济学\n\n经济学是一门对产品和服务的生产、分配以及消费进行研究的社会科学。西方语言中的“经济学”一词源于古希腊的。\n\n经济学注重的是研究经济行为者在一个经济体系下的行为，以及他们彼此之间的互动。在现代，经济学的教材通常将这门领域的研究分为总体经济学和个体经济学。微观经济学检视一个社会里基本层次的行为，包括个体的行为者（例如个人、公司、买家或卖家）以及与市场的互动。而宏观经济学则分析整个经济体和其议题，包括失业、通货膨胀、经济成长、财政和货币政策等。..."}

#### 效果：

    经济学
    经济学是一门对产品和服务的生产、分配以及消费进行研究的社会科学。西方语言中的“经济学”一词源于古希腊的。
    经济学注重的是研究经济行为者在一个经济体系下的行为，以及他们彼此之间的互动。在现代，经济学的教材通常将这门领域的研究分为总体经济学和个体经济学。微观经济学检视一个社会里基本层次的行为，包括个体的行为者（例如个人、公司、买家或卖家）以及与市场的互动。而宏观经济学则分析整个经济体和其议题，包括失业、通货膨胀、经济成长、财政和货币政策等。
    其他的对照还包括了实证经济学（研究「是什么」）以及规范经济学（研究「应该是什么」）、经济理论与实用经济学、行为经济学与理性选择经济学、主流经济学（研究理性-个体-均衡等）与非主流经济学（研究体制-历史-社会结构等）。
    经济学的分析也被用在其他各种领域上，主要领域包括了商业、金融、和政府等，但同时也包括了如健康、犯罪、教育、法律、政治、社会架构、宗教、战争、和科学等等。到了21世纪初，经济学在社会科学领域各方面不断扩张影响力，使得有些学者讽刺地称其为「经济学帝国主义」。
    在现代对于经济学的定义有数种说法，其中有许多说法因为发展自不同的领域或理论而有截然不同的定义，苏格兰哲学家和经济学家亚当·斯密在1776年将政治经济学定义为「国民财富的性质和原因的研究」，他说：
    让-巴蒂斯特·赛伊在1803年将经济学从公共政策里独立出来，并定义其为对于财富之生产、分配、和消费的学问。另一方面，托马斯·卡莱尔则讽刺的称经济学为「忧郁的科学」（Dismal science），不过这一词最早是由马尔萨斯在1798年提出。约翰·斯图尔特·密尔在1844年提出了一个以社会科学定义经济学的角度：
    .....

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/img/wiki_zh.jpg"  width="90%" height="90%" />

<br>

2.新闻语料json版(news2016zh)
-------------------------------------------------------------------------

#### 250万篇新闻( 原始数据9G，压缩文件3.6G；新闻内容跨度：2014-2016年)

<a href='https://drive.google.com/file/d/1TMKu1FpTr6kcjWXWlQHX7YJsMfhhcVKp/view?usp=sharing'>Google Drive下载</a>或 <a href='https://pan.baidu.com/s/1MLLM-CdM6BhJkj8D0u3atA'>百度云盘下载</a>，密码:k265

#### 数据描述

包含了250万篇新闻。新闻来源涵盖了6.3万个媒体，含标题、关键词、描述、正文。

数据集划分：数据去重并分成三个部分。训练集：243万；验证集：7.7万；测试集，数万，不提供下载。

#### 可能的用途：

    可以做为【通用中文语料】，训练【词向量】或做为【预训练】的语料；
   
    也可以用于训练【标题生成】模型，或训练【关键词生成】模型（选关键词内容不同于标题的数据）；

    亦可以通过新闻渠道区分出新闻的类型。

#### 结构：

    {'news_id': <news_id>,'title':<title>,'content':<content>,'source': <source>,'time':<time>,'keywords': <keywords>,'desc': <desc>, 'desc': <desc>}

    其中，title是新闻标题，content是正文，keywords是关键词，desc是描述，source是新闻的来源，time是发布时间

#### 例子：
    
    {"news_id": "610130831", "keywords": "导游，门票","title": "故宫淡季门票40元 “黑导游”卖外地客140元", "desc": "近日有网友微博爆料称，故宫午门广场售票处出现“黑导游”，专门向外地游客出售高价门票。昨日，记者实地探访故宫，发现“黑导游”确实存在。窗口出售", "source": "新华网", "time": "03-22 12:00", "content": "近日有网友微博爆料称，故宫午门广场售票处出现“黑导游”，专门向外地游客出售高价门票。昨日，记者实地探访故宫，发现“黑导游”确实存在。窗口出售40元的门票，被“黑导游”加价出售，最高加到140元。故宫方面表示，请游客务必通过正规渠道购买门票，避免上当受骗遭受损失。目前单笔门票购买流程不过几秒钟，耐心排队购票也不会等待太长时间。....再反弹”的态势，打击黑导游需要游客配合，通过正规渠道购买门票。"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/img/news2016zh.png"  width="100%" height="100%" />

<br>

3.百科类问答json版(baike2018qa)
-------------------------------------------------------------------------

#### 150万个问答( 原始数据1G多，压缩文件663M；数据更新时间：2018年)

<a href="https://drive.google.com/open?id=1_vgGQZpfSxN_Ng9iTAvE7hM3Z7NVwXP2">Google Drive下载</a> 或 <a href='https://pan.baidu.com/s/12TCEwC_Q3He65HtPKN17cA'>百度云盘下载</a>，密码:fu45


#### 数据描述

含有150万个预先过滤过的、高质量问题和答案，每个问题属于一个类别。总共有492个类别，其中频率达到或超过10次的类别有434个。

数据集划分：数据去重并分成三个部分。训练集：142.5万；验证集：4.5万；测试集，数万，不提供下载。

#### 可能的用途：

    可以做为通用中文语料，训练词向量或做为预训练的语料；也可以用于构建百科类问答；其中类别信息比较有用，可以用于做监督训练，从而构建

    更好句子表示的模型、句子相似性任务等。

#### 结构：

    {"qid":<qid>,"category":<category>,"title":<title>,"desc":<desc>,"answer":<answer>}
    
    其中，category是问题的类型，title是问题的标题，desc是问题的描述，可以为空或与标题内容一致。

#### 例子：
    
    {"qid": "qid_2540946131115409959", "category": "生活知识", "title": "冬天进补好一些呢，还是夏天进步好啊？ ", "desc": "", "answer": "你好！\r\r当然是冬天进补好的了，夏天人体的胃处于收缩状态，不适宜大量的进补，所以我们有时候说：“夏天就要吃些清淡的，就是这个道理的。”\r\r不过，秋季进补要注意“四忌” 一忌多多益善。任何补药服用过量都有害。认为“多吃补药，有病治病，无病强身”是不的。过量进补会加重脾胃、肝脏负担。在夏季里，人们由于喝冷饮，常食冻品，多有脾胃功能减弱的现象，这时候如果突然大量进补，会骤然加重脾胃及肝脏的负担，使长期处于疲弱的消化器官难于承受，导致消化器官功能紊乱。 \r\r二忌以药代食。重药物轻食物的做法是不科学的，许多食物也是好的滋补品。如多吃荠菜可治疗高血压；多吃萝卜可健胃消食，顺气宽胸；多吃山药能补脾胃。日常食用的胡桃、芝麻、花生、红枣、扁豆等也是进补的佳品。\r\r三忌越贵越好。每个人的身体状况不同，因此与之相适应的补品也是不同的。价格昂贵的补品如燕窝、人参之类并非对每个人都适合。每种进补品都有一定的对象和适应症，应以实用有效为滋补原则，缺啥补啥。 \r\r四忌只补肉类。秋季适当食用牛羊肉进补效果好。但经过夏季后，由于脾胃尚未完全恢复到正常功能，因此过于油腻的食品不易消化吸收。另外，体内过多的脂类、糖类等物质堆积可能诱发心脑血管病。"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/img/baike_qa.png"  width="100%" height="100%" />

#### 公开评测：

欢迎报告模型在验证集上的准确率。任务1： 类别预测。

报告包括：#1）验证集上准确率；#2）采用的模型、方法描述、运行方式，1页PDF；#3）可运行的源代码(可选)

基于#2和#3，我们会在测试集上做测试，并报告测试集上的准确率；只提供了#1和#2的队伍，验证集上的成绩依然可以被显示出来，但会被标记为未验证。


<br>

4.社区问答json版(webtext2019zh) ：大规模高质量数据集
-------------------------------------------------------------------------

#### 410万个问答( 过滤后数据3.7G，压缩文件1.7G；数据跨度：2015-2016年)

<a href='https://drive.google.com/open?id=1u2yW_XohbYL2YAK6Bzc5XrngHstQTf0v'>Google Drive下载</a>


#### 数据描述

含有410万个预先过滤过的、高质量问题和回复。每个问题属于一个【话题】，总共有2.8万个各式话题，话题包罗万象。

从1400万个原始问答中，筛选出至少获得3个点赞以上的的答案，代表了回复的内容比较不错或有趣，从而获得高质量的数据集。

除了对每个问题对应一个话题、问题的描述、一个或多个回复外，每个回复还带有点赞数、回复ID、回复者的标签。

数据集划分：数据去重并分成三个部分。训练集：412万；验证集：6.8万；测试集a：6.8万；测试集b，不提供下载。


#### 可能的用途：
    
    1）构建百科类问答：输入一个问题，构建检索系统得到一个回复或生产一个回复；或根据相关关键词从，社区问答库中筛选出你相关的领域数据
    
    2）训练话题预测模型：输入一个问题(和或描述)，预测属于话题。
    
    3）训练社区问答(cQA)系统：针对一问多答的场景，输入一个问题，找到最相关的问题，在这个基础上基于不同答案回复的质量、
    
      问题与答案的相关性，找到最好的答案。

    4）做为通用中文语料，做大模型预训练的语料或训练词向量。其中类别信息也比较有用，可以用于做监督训练，从而构建更好句子表示的模型、句子相似性任务等。
    
    5）结合点赞数量这一额外信息，预测回复的受欢迎程度或训练答案评分系统。

#### 结构：

    {"qid":<qid>,"title":<title>,"desc":<desc>,"topic":<topic>,"star":<star>,"content":<content>,
    
    "answer_id":<answer_id>,"answerer_tags":<answerer_tags>}
    
    其中，qid是问题的id，title是问题的标题，desc是问题的描述，可以为空；topic是问题所属的话题，star是该回复的点赞个数，
    
    content是回复的内容，answer_id是回复的ID,answerer_tags是回复者所携带的标签

#### 例子：
    
    {"qid": 65618973, "title": "AlphaGo只会下围棋吗？阿法狗能写小说吗？", "desc": "那么现在会不会有智能机器人能从事文学创作？<br>如果有，能写出什么水平的作品？", "topic": "机器人", "star": 3, "content": "AlphaGo只会下围棋，因为它的设计目的，架构，技术方案以及训练数据，都是围绕下围棋这个核心进行的。它在围棋领域的突破，证明了深度学习深度强化学习MCTS技术在围棋领域的有效性，并且取得了重大的PR效果。AlphaGo不会写小说，它是专用的，不会做跨出它领域的其它事情，比如语音识别，人脸识别，自动驾驶，写小说或者理解小说。如果要写小说，需要用到自然语言处理（NLP））中的自然语言生成技术，那是人工智能领域一个", "answer_id": 545576062, "answerer_tags": "人工智能@游戏业"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/img/webtext2019zh.png"  width="100%" height="100%" />


#### 在该数据集上的公开评测和任务：

任务1： 话题预测。

报告包括：#1）验证集上准确率；#2）采用的模型、方法描述、运行方式，1页PDF；#3）可运行的源代码(可选)

基于#2和#3，我们会在测试集上做测试，并报告测试集上的准确率；只提供了#1和#2的队伍，验证集上的成绩依然可以被显示出来，但会被标记为未验证。

任务2：训练社区问答(cQA)系统。

要求：评价指标采用MAP，构建一个适合排序问题的测试集，并报告在该测试集上的效果。

任务3：使用该数据集（webtext2019zh)，参考OpenAI的GPT-2，训练中文的文本写作模型、测试在其他数据集上的zero-shot的效果，或测评语言模型的效果。

<br>


5.翻译语料(translation2019zh)
-------------------------------------------------------------------------

#### 520万个中英文平行语料( 原始数据1.1G，压缩文件596M)

<a href='https://drive.google.com/open?id=1EX8eE5YWBxCaohBO8Fh4e2j3b9C2bTVQ'>Google Drive下载</a>


#### 数据描述

中英文平行语料520万对。每一个对，包含一个英文和对应的中文。中文或英文，多数情况是一句带标点符号的完整的话。

对于一个平行的中英文对，中文平均有36个字，英文平均有19个单词(单词如“she”)

数据集划分：数据去重并分成三个部分。训练集：516万；验证集：3.9万；测试集，数万，不提供下载。

#### 可能的用途：
    
    可以用于训练中英文翻译系统，从中文翻译到英文，或从英文翻译到中文；
    
    由于有上百万的中文句子，可以只抽取中文的句子，做为通用中文语料，训练词向量或做为预训练的语料。英文任务也可以类似操作；
    

#### 结构：

    {"english": <english>, "chinese": <chinese>}
    
    其中，english是英文句子，chinese是中文句子，中英文一一对应。

#### 例子：
    
    {"english": "In Italy, there is no real public pressure for a new, fairer tax system.", "chinese": "在意大利，公众不会真的向政府施压，要求实行新的、更公平的税收制度。"}
  

<img src="https://github.com/brightmart/nlp_chinese_corpus/blob/master/resources/img/translation2019zh.jpeg"  width="100%" height="100%" />


贡献语料/Contribution
-------------------------------------------------------------------------

贡献中文语料，请发送邮件至nlp_chinese_corpus@163.com

为了共同建立一个大规模开放共享的中文语料库，以促进中文自然语言处理领域的发展，凡提供语料并被采纳到该项目中，

除了会列出贡献者名单（可选）外，我们会根据语料的质量和量级，选出前20个同学，结合您的意愿，寄出键盘、鼠标、

显示屏、无线耳机、智能音箱或其他等值的物品，以表示对贡献者的感谢。

add your chinese corpus here by sending us an email

if there is any issue regarding the data, you can also contact with us, we will process it within one week. 

thank you for your understanding.


项目贡献者或组织清单
-------------------------------------------------------------------------

1. <a href='https://github.com/ReactiveCJ'>ReactiveCJ</a>


引用 Citation / How do I cite Us?
-------------------------------------------------------------------------

    @misc{bright_xu_2019_3402023,
    author       = {Bright Xu},
    title        = {NLP Chinese Corpus: Large Scale Chinese Corpus for NLP },
    month        = sep,
    year         = 2019,
    doi          = {10.5281/zenodo.3402023},
    version      = {1.0},
    publisher    = {Zenodo},
    url          = {https://doi.org/10.5281/zenodo.3402023}
    }


<a href="https://zenodo.org/badge/latestdoi/169745123"><img src="https://zenodo.org/badge/169745123.svg" alt="DOI"></a>

也请发邮件告知我们您的论文名称或在这个项目的数据集上的工作


贡献中文语料，请发送邮件: CLUEbenchmark@163.com；

Reference
-------------------------------------------------------------------------

1. <a href='https://github.com/AimeeLee77/wiki_zh_word2vec'>利用Python构建Wiki中文语料词向量模型试验</a>

2. <a href='https://github.com/attardi/wikiextractor'>A tool for extracting plain text from Wikipedia dumps</a>

3. <a href='https://github.com/yichen0831/opencc-python'>Open Chinese convert (OpenCC) in pure Python:開放中文轉換</a>

4. <a href='https://dumps.wikimedia.org/zhwiki/latest/'>dumps of wiki, latest in chinese</a>


