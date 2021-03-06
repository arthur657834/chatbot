```
CC是连接词
RB是副词
IN是介词
NN是名次
JJ是形容词
VBP是动词
PRO是代词
```

### 词性标注:
1. 默认标注器
2. 正则表达式标注器
3. 查询标注器
  * 3.1  一元标注：基于已经标注的语料库做训练，然后用训练好的模型来标注新的语料
  * 3.2 二元标注和多元标注：一元标注指的是只考虑当前这个词，不考虑上下文。二元标注器指的是考虑它前面的词的标注
4. 组合标注器：为了提高精度和覆盖率，我们对多种标注器组合，比如组合二元标注器、一元标注器和默认标注器，如下：  

机器学习的过程是训练模型和使用模型的过程，训练就是基于已知数据做统计学习，使用就是用统计学习好的模型来计算未知的数据。

机器学习分为有监督学习和无监督学习，文本分类也分为有监督的分类和无监督的分类。有监督就是训练的样本数据有了确定的判断，基于这些已有的判断来断定新的数据，无监督就是训练的样本数据没有什么判断，完全自发的生成结论。

文本分类除了文档分类外还有许多其他类型的分类，比如：

词性标注：属于一种文本分类，一般是基于上下文语境的文本分类

句子分割：属于标点符号的分类任务，它的特征一般选取为单独句子标识符的合并链表、数据特征（下一个词是否大写、前一个词是什么、前一个词长度……）

识别对话行为类型：对话行为类型是指问候、问题、回答、断言、说明等

识别文字蕴含：即一个句子是否能得出另外一个句子的结论，这可以认为是真假标签的分类任务。这是一个有挑战的事情

任何语言的每一句话之所以称为“话”，是因为它有一定的句子结构，除了一个个独立的词之外，他们之间还存在着某种关系。如果任何一句话可以由任何词构成，可长可短，那么这是一个非结构化的信息，计算机是很难理解并做计算的，但是如果能够以某种方式把句子转化成结构化的形式，计算机就可以理解了。

断句、分词、词性标注、分块

可以采用IOB标记，I(inside，内部)、O(outside，外部)、B(begin, 开始)，一个块的开始标记为B，块内的标识符序列标注为I，所有其他标识符标注为O

也可以用树结构来存储分块

通过上面的分块可以很容易识别出实体，那么关系抽取实际就是找出实体和实体之间的关系，
