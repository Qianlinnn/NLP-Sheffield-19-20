<<<<<<< HEAD

=======
>>>>>>> 93acafe8c628f3c31b4fed7eda3eba417ac9dbf7
# Text units
* **word**(**token/term**): 一个或者多个不包含空格的字符序列。有时候还会包括n-grams
* **document(text sequence/snippet)** 句子，段落，社交媒体帖子等

## Document-Word Matrix(文档-文字矩阵)
* 一个矩阵 X, |*D*|X|*V*| 行是在语料库里*D*的的文档个数， 列是在*V*里面的词汇表
* 每一个文档，都要计算属于词汇表的单词出现了多少次
* X也可以把文档中所有文字的one-hot 向量相加然后转置他们
      
# Label 种类
* 积极的或消极的 
* 主题（如运动 政策）
* 作者名字
* 在文章打分时是通过还是fail
* 是否支持立场(stance)
* 具有有限类集的任何人物

## 把label更抽象一点
* binary(0 or 1),如该电影评论是积极的还是消极的
* multi-class(1 out of k classes)如一个新闻文章的主题是什么（从运动，政策，商务，科技里选）
* multi-label(n out of k classes)这个新闻可能涉及到多个领域，可能是运动政策等等
* real number， 预测一个电影的评分是多少，我们通常叫他回归

# 文本类型(Text types)