# Awesome Chinese Corpus, Datasets and Models

This tutorial is aimed to collect corpus, datasets, and models for Chinese information processing.

[TOC] Outline

## 1. Corpus

### 1.1 Wikipedia Chinese

Download address: [BaiduNets](https://pan.baidu.com/s/1uPMlIY3vhusdnhAge318TA)

Reference: [Github](https://github.com/brightmart/nlp_chinese_corpus)

Format: JSON file. 

Example: It contains 1,000,000+ items. 
```
{
    "id": "53", 
    "url": "https://zh.wikipedia.org/wiki?curid=53", 
    "title": "经济学", 
    "text": "经济学\n\n经济学是一门对产品和服务的生产、分配以及消费进行研究的社会科学。西方
    语言中的“经济学”一词源于..."
}
{
    "id": "123", 
    "url": "https://zh.wikipedia.org/wiki?curid=123", 
    "title": "xxx", 
    "text": "xxx..."
}
```


## 1.2 Chinese News

Download address: [BaiduNets](https://drive.google.com/file/d/1TMKu1FpTr6kcjWXWlQHX7YJsMfhhcVKp/view?usp=sharing)

Reference: [Github](https://github.com/brightmart/nlp_chinese_corpus)

Format: JSON file. 

Example: It contains 2,500,000+ items, like
```
{
    "news_id": "610130831", 
    "keywords": "导游，门票",
    "title": "故宫淡季门票40元 “黑导游”卖外地客140元", 
    "desc": "近日有网友微博爆料称，故宫午门广场售票处出现“黑导游”，专门向外地游客出售高价门票。
    昨日，记者实地....。"
}
{
    "news_id": "910130831", 
    "keywords": "yyy，xxx",
    "title": "xxxxxxx", 
    "desc": "..."
}
```


## 2 Dictionary

### 2.1 China Xinhua dictionary

This dictionary includes 14032 Xiehouyu, 31648 idioms, 264434 words, 16142 Chinese characters.


Download address: [Github](https://github.com/pwxcoo/chinese-xinhua/archive/master.zip)

Reference: [Github](https://github.com/pwxcoo/chinese-xinhua)

Format: JSON file. 

Example: 
It contains 264434 idioms which like
<pre>
<code>
[
    {
        "derivation": "语出《法华经·法师功德品》下至阿鼻地狱。”",
        "example": "但也有少数意志薄弱的……逐步上当，终至堕入～。★《上饶集中营·炼狱杂记》",
        "explanation": "阿鼻梵语的译音，意译为无间”，即痛苦无有间断之意。常用来比喻黑暗的社会和严酷的牢狱。又比喻无法摆脱的极其痛苦的境地。",
        "pinyin": "ā bí dì yù",
        "word": "阿鼻地狱",
        "abbreviation": "abdy"
    },
    ...
]
</code>
</pre>

It contains 264434 words which like
<pre>
<code>
[
    { 
        "ci": "宸纶", 
        "explanation": "1.帝王的诏书﹑制令。" 
    },
    ...
]
</code>
</pre>

It contains 16142 characters which like
<pre>
<code>
[
    {
        "word": "嗄",
        "oldword": "嗄",
        "strokes": "13",
        "pinyin": "á",
        "radicals": "口",
        "explanation": "嗄〈叹〉\n\n 同啊”。表示省悟或惊奇\n\n 嗄!难道这里是没有地方官的么?--宋·佚名《新编五代史平话》\n\n 嗄á叹词。在句首，〈表〉疑问或反问～，这是什么？～，你想干什么？\"嗄\"另见shà㈠。\n\n 嗄shà\n\n ⒈声音嘶哑～声。\n\n 嗄a 1.助词。表示强调﹑肯定或辩解。 2.助词。方言。表示疑问或反诘。\n\n 嗄xià 1.见\"嗄饭\"。 2.见\"嗄程\"。",
        "more": "嗄 ga、a 部首 口 部首笔画 03 总笔画 13  嗄2\nshà\n〈形〉\n(1)\n声音嘶哑的 [hoarse]\n终日嚎而嗌不嗄。--《老子》\n(2)\n又如嗄哑,嗄嘶(嗓音嘶哑)\n嗄\nshà\n〈叹〉\n(1)\n什么 [what]--表示否定\n我要丢个干干净,看你嗄法把我治。--清·蒲松龄《聊斋俚曲集》\n(2)\n旧时仆役对主人、下级对上级的应诺声 [yes]\n带进来”。两边军士应一声嗄”,即将牛皋推至面前。--《说岳全传》\n另见á\n嗄1\ná\n〈叹〉\n同啊”(á)。表示省悟或惊奇 [ah]\n嗄!难道这里是没有地方官的么?--宋·佚名《新编五代史平话》\n另见shà\n嗄1\nshà　ㄕㄚ╝\n嗓音嘶哑。\n郑码janr，u55c4，gbke0c4\n笔画数13，部首口，笔顺编号2511325111354\n嗄2\ná　ㄚˊ\n同啊2”。\n郑码janr，u55c4，gbke0c4\n笔画数13，部首口，笔顺编号2511325111354"
    },
    ... 
]
</code>
</pre>

It contains 14032 Xiehouyu which like
<pre>
<code>
[
    {
        "riddle": "飞机上聊天",
        "answer": "高谈阔论"
    },
    ...
]
</code>
</pre>

## 3. Datasets

### 3.1 Machine reading comprehension datasets

#### 3.1.1 CMRC-2018: Chinese Machine Reading Comprehension (CMRC) 2018 Public Dataset

[The Second Evaluation Workshop on Chinese Machine Reading Comprehension](https://hfl-rc.github.io/cmrc2018) was successfully ended. The evaluation committee had decided to continue to accept submissions to further test their systems on the hidden test set and challenge set. 

Open Challenge Leaderboard: [https://hfl-rc.github.io/cmrc2018/open_challenge/](https://hfl-rc.github.io/cmrc2018/open_challenge/)

Reference: 
System overview: [https://arxiv.org/abs/1810.07366](https://arxiv.org/abs/1810.07366)

If you wish to use this data in your research, please cite:
<pre>
<code>
@article{cmrc2018-dataset,
    title={A Span-Extraction Dataset for Chinese Machine Reading Comprehension},
    author={Cui, Yiming and Liu, Ting and Xiao, Li and Chen, Zhipeng and Ma, Wentao and Che, Wanxiang and Wang, Shijin and Hu, Guoping},
    journal={arXiv preprint arXiv:1810.07366},
    year={2018}
}
</code>
</pre>

##### Original Data

These are the original CMRC 2018 public data.

uuid[0:8]	|name	|summary	|data_size	|state	|description
 ----- | ----- | ------ | ----- | ------ | ------------- 
0x0e6dce	|[cmrc2018_evaluate.py](https://worksheets.codalab.org/rest/bundles/0x0e6dced40a0d40d980da88882aa8c13a/contents/blob/)	|[uploaded]	|4.1k	|ready	|CMRC 2018 Official Evaluation Script v5
0xcd4c75	|[cmrc2018_trial.json](https://worksheets.codalab.org/rest/bundles/0xcd4c755829064426896ef942a249aced/contents/blob/)	|[uploaded]	|1.0m	|ready	|CMRC 2018 Trial Data
0x296baa	|[cmrc2018_train.json](https://worksheets.codalab.org/rest/bundles/0x296baa11dfbc4ab08cdeb5b4adf182e2/contents/blob/)	|[uploaded]	|9.0m	|ready	|CMRC 2018 Training Data
0xb70e5e	|[cmrc2018_dev.json](https://worksheets.codalab.org/rest/bundles/0xb70e5e281fcd437d9aa8f1c4da107ae4/contents/blob/)	|[uploaded]	|3.4m	|ready	|CMRC 2018 Development Data


##### SQuAD-style Data

As our data is a little bit different from SQuAD dataset in terms of the name of the key. If you wish to use exactly the same format as SQuAD, please download the following converted data and evaluation script. Note that, the content is exactly the same with the original CMRC 2018 data.

uuid[0:8]	|name	|summary	|data_size	|state	|description
 ----- | ----- | ------ | ----- | ------ | ------------- 
0x1ecd59	|[cmrc2018_evaluate.py](https://worksheets.codalab.org/rest/bundles/0x1ecd59f275a64bbd8cd79868ed059204/contents/blob/)	|[uploaded]	|4.2k	|ready	|CMRC 2018 Official Evaluation Script v5-sp
0x182c2e	|[cmrc2018_trial.json](https://worksheets.codalab.org/rest/bundles/0x182c2e71fac94fc2a45cc1a3376879f7/contents/blob/)	|[uploaded]	|781k	|ready	|CMRC 2018 Trial Data (SQuAD-style)
0x15022f	|[cmrc2018_train.json](https://worksheets.codalab.org/rest/bundles/0x15022f0c4d3944a599ab27256686b9ac/contents/blob/)	|[uploaded]	|7.1m	|ready	|CMRC 2018 Training Data (SQuAD-style)
0x722526	|[cmrc2018_dev.json](https://worksheets.codalab.org/rest/bundles/0x72252619f67b4346a85e122049c3eabd/contents/blob/)	|[uploaded]	|3.1m	|ready	|CMRC 2018 Development Data (SQuAD-style)



### 3.2 Question-asnwering datasets

#### 3.2.1 Baike

Download address: [BaiduNets](https://pan.baidu.com/s/12TCEwC_Q3He65HtPKN17cA) 
(Extract code can be find in the following references.)

Reference: [Github](https://github.com/brightmart/nlp_chinese_corpus)

Format: Json file. 

Example: It contains 1,500,000 questions, like
<pre>
<code>
{
    "qid": "qid_2540946131115409959", 
    "category": "生活知识", 
    "title": "冬天进补好一些呢，还是夏天进步好啊？ ", 
    "desc": "", 
    "answer": "你好！\r\r当然是冬天进补好的了，夏天人体的胃处于收缩状态，不适宜大量的进补，所以我们
    有时候说：“夏天就要吃些清淡的，就是这个道理的。”\r\r不过，秋季进补要注意“四忌” 一忌多多益善。任
    何补药服用过量都有害。认为“多吃补药，有病治病，无病强身”是不的。过量进补会加重脾胃、肝脏负担。在
    夏季里，人们由于喝冷饮，常食冻品，多有脾胃功能减弱的现象，这时候如果突然大量进补，会骤然加重脾胃
    及肝脏的负担，使长期处于疲弱的消化器官难于承受，导致消化器官功能紊乱。 \r\r二忌以药代食。重药物
    轻食物的做法是不科学的，许多食物也是好的滋补品。如多吃荠菜可治疗高血压；多吃萝卜可健胃消食，顺气
    宽胸；多吃山药能补脾胃。日常食用的胡桃、芝麻、花生、红枣、扁豆等也是进补的佳品。\r\r三忌越贵越
    好。每个人的身体状况不同，因此与之相适应的补品也是不同的。价格昂贵的补品如燕窝、人参之类并非对每
    个人都适合。每种进补品都有一定的对象和适应症，应以实用有效为滋补原则，缺啥补啥。 \r\r四忌只补肉
    类。秋季适当食用牛羊肉进补效果好。但经过夏季后，由于脾胃尚未完全恢复到正常功能，因此过于油腻的
    食品不易消化吸收。另外，体内过多的脂类、糖类等物质堆积可能诱发心脑血管病。"
}
{
    "qid": "qid_2540946131115484405", 
    "category": "生活知识", 
    "title": "冬天应该睡多久？ ", 
    "desc": "", 
    "answer": "你好！\r\r当然是冬天..."
}
</code>
</pre>

This dataset can also be used for training word-embeddings.

#### 3.2.2 Web question-answering

Download address: [Google Disk](https://drive.google.com/open?id=1u2yW_XohbYL2YAK6Bzc5XrngHstQTf0v)

Reference: [Github](https://github.com/brightmart/nlp_chinese_corpus)

Format: Json file. 

Example: It contains 4,100,000 questions, like
<pre>
<code>
{
    "qid": 65618973, 
    "title": "AlphaGo只会下围棋吗？阿法狗能写小说吗？", 
    "desc": "那么现在会不会有智能机器人能从事文学创作？<br>如果有，能写出什么水平的作品？", 
    "topic": "机器人", 
    "star": 3, 
    "content": "AlphaGo只会下围棋，因为它的设计目的，架构，技术方案以及训练数据，都是围绕下
    围棋这个核心进行的。它在围棋领域的突破，证明了深度学习深度强化学习MCTS技术在围棋领域的有
    效性，并且取得了重大的PR效果。AlphaGo不会写小说，它是专用的，不会做跨出它领域的其它事情，
    比如语音识别，人脸识别，自动驾驶，写小说或者理解小说。如果要写小说，需要用到自然语言处
    理（NLP））中的自然语言生成技术，那是人工智能领域一个", 
    "answer_id": 545576062, 
    "answerer_tags": "人工智能@游戏业"
}
{
    "qid": 65612373, 
    "title": "AlphaGo只会下蛋吗？阿法狗会咬人吗？", 
    "desc": "", 
    "topic": "机器人", 
    "star": 3, 
    "content": "..."
    "answer_id": 545576062, 
    "answerer_tags": "人工智能@游戏业"
}
</code>
</pre>

This dataset can also be used for training word-embeddings.

### 3.3 Translation datasets

#### 3.3.1 English <> Chinese translation

Download address: [Google Disk](https://drive.google.com/open?id=1EX8eE5YWBxCaohBO8Fh4e2j3b9C2bTVQ)

Reference: [Github](https://github.com/brightmart/nlp_chinese_corpus)

Format: Json file. 

Example: It contains 5,200,000 pairs, like
<pre>
<code>
{
    "english": "In Italy, there is no real public pressure for a new, fairer tax system.", 
    "chinese": "在意大利，公众不会真的向政府施压，要求实行新的、更公平的税收制度。"
}
{
    "english": "Hello, how are you?", 
    "chinese": "喂，你好吗？"
}
</code>
</pre>


### 3.4 Translation datasets

## 4. Models

### 4.1 Chinese-BERT-wwm

State of the art results on [CMRC-2018]()

Code: [Github](https://github.com/ymcui/Chinese-BERT-wwm)







