pip install nltk

python
    import nltk
    nltk.download()
        d
        [*] book

from nltk.book import *
        
text1
text1.concordance("former")        
text1.similar("ship")
text4.dispersion_plot(["citizens", "democracy", "freedom", "duties", "America"])


len(text1)：返回总字数

set(text1)：返回文本的所有词集合

len(set(text4))：返回文本总词数

text4.count("is")：返回“is”这个词出现的总次数

FreqDist(text1)：统计文章的词频并按从大到小排序存到一个列表里

fdist1 = FreqDist(text1);fdist1.plot(50, cumulative=True)：统计词频，并输出累计图像

fdist1.hapaxes()：返回只出现一次的词

text4.collocations()：频繁的双联词


自然语言处理分两派:
基于规则的,也就是完全从语法句法等出发
基于统计