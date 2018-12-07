[toc]
# 介绍

## Elasticsearch 与Lucene

Elasticsearch是一个基于[Apache Lucene(TM)](https://lucene.apache.org/core/)的开源搜索引擎。无论在开源还是专有领域，Lucene可以被认为是迄今为止最先进、性能最好的、功能最全的搜索引擎库。

但是，Lucene只是一个库。想要使用它，你必须使用Java来作为开发语言并将其直接集成到你的应用中，更糟糕的是，Lucene非常复杂，你需要深入了解检索的相关知识来理解它是如何工作的。

Elasticsearch使用Lucene作为其核心，实现索引和搜索的功能，但是它的目的是通过简单的`RESTful API`来隐藏Lucene的复杂性，从而让全文搜索变得简单。



## Elasticsearch解决的痛点

现在大部分数据库在提取可用知识方面显得异常无能。它们能够通过时间戳或者精确匹配做过滤，但是它们能够进行全文搜索，处理同义词和根据相关性给文档打分吗？它们能根据同一份数据生成分析和聚合的结果吗？最重要的是，它们在没有大量工作进程（线程）的情况下能做到对数据的实时处理吗？

这就是Elasticsearch存在的理由：Elasticsearch鼓励你浏览并利用你的数据，而不是让它烂在数据库里，因为在数据库里实在太难查询了。



## Elastichsearch特性

- 分布式的实时文件存储，每个字段都被索引并可被搜索
- 分布式的实时分析搜索引擎
- 可以扩展到上百台服务器，处理PB级结构化或非结构化数据

------

- 上手容易。对初学者隐藏了复杂的搜索引擎理论。可以通过简单的`RESTful API`、各种语言的客户端甚至命令行与之交互。
- 随着你对Elasticsearch的理解加深，你可以根据不同的问题领域定制Elasticsearch的高级特性
- Elasticsearch在[Apache 2 license](http://www.apache.org/licenses/LICENSE-2.0.html)下许可使用，可以免费下载、使用和修改。



## 使用Elasticsearch的公司

它可用于全文搜索、结构化搜索、分析或将这三者混合使用：

- 维基百科使用Elasticsearch提供全文搜索并高亮关键字，以及**输入实时搜索(search-as-you-type)**和**搜索纠错(did-you-mean)**等搜索建议功能。
- 英国卫报使用Elasticsearch结合用户日志和社交网络数据提供给他们的编辑以实时的反馈，以便及时了解公众对新发表的文章的回应。
- StackOverflow结合全文搜索与地理位置查询，以及**more-like-this**功能来找到相关的问题和答案。
- `Github`使用Elasticsearch检索**1300亿行**的代码。

Elasticsearch不仅用于大型企业，它还可以让初创公司将最初的想法变成可扩展的解决方案。Elasticsearch可以在你的笔记本上运行，也可以在数以百计的服务器上处理PB级别的数据。





## 小结

Elasticsearch所涉及到的每一项技术都不是创新或者革命性的，全文搜索，分析系统以及分布式数据库这些早就已经存在了。它的革命性在于将这些独立且有用的技术整合成一个一体化的、实时的应用。它对新用户的门槛很低，当然它也会跟上你技能和需求增长的步伐。

