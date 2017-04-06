Gutenberg语料库:
nltk.corpus.gutenberg就是gutenberg语料库的阅读器，它有很多实用的方法，比如：

nltk.corpus.gutenberg.raw('chesterton-brown.txt')：输出chesterton-brown.txt文章的原始内容

fileids()：返回语料库中的文件

categories()：返回语料库中的分类

words()：返回语料库中的词汇

sents()：返回语料库句子

abspath()：指定文件在磁盘上的位置

open()：打开语料库的文件流

类似的语料库还有：

from nltk.corpus import webtext：网络文本语料库，网络和聊天文本

from nltk.corpus import brown：布朗语料库，按照文本分类好的500个不同来源的文本

from nltk.corpus import reuters：路透社语料库，1万多个新闻文档

from nltk.corpus import inaugural：就职演说语料库，55个总统的演说

语料库的一般结构：
* 散养式（孤立的多篇文章）
* 分类式（按照类别组织，相互之间没有交集）
* 交叉式（一篇文章可能属于多个类）
* 渐变式（语法随着时间发生变化）
