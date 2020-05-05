# python-datascience-sklearn-deeplearning

在未来的很长一段时间里，介绍python数据科学完整的学习路线，以及自我的学习经历。欢迎Fork

####  numpy and pandas 

numpy和pandas作为数据处理两个最基本的package，也是整个学习路线最为重要的一环。简单来说，numpy是针对array的学习，而pandas针对Series和DataFrame,两个数据结构。在np&pandas中，我上传 《利用python进行数据分析》第二版，这本书的大名我也不过多介绍。在我整个学习过程中，如何熟练掌握这些复杂的函数和使用规则，关键在于使用的频率。一个很简单的问题，关于两个CSV文件合并的问题，常见的含有merge，concat，join函数，如何根据已有的数据进行分组合并，这个时候我们就可能遇到一个问题，缺失值的处理，在通常情况下。

```python
import pandas as pd
dataset.dropna(how='any',axis=0,inplace=True)
```

似乎能解决所有的问题，但是存在相当大的可能性，你会数据集压缩至非常小的程度,这个时候，如何做呢

```python
dataset.dropna(thesh=number)#或者这种
dataset.fillna()#这种补0的方法，可以使用拉格朗日插值的方法，或者在sklearn Imupter有更多的可能性
```