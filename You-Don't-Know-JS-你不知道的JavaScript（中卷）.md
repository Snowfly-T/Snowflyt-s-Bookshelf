# You Don't Know JS - 你不知道的JavaScript（中卷）

## 图书信息

- 英文书名：You Don't Know JS: Types & Grammar & Async & Performance
- 中文书名：你不知道的 JavaScript（中卷）
- 作者：[美] Kyle Simpson
- 译者：单业 / 姜南
- 页数：正文 307 页 / 附录 51 页
- 英文出版社：O'Reilly Media
- 中文出版社：人民邮电出版社 / 图灵教育
- 出版日期：英文原版 2015 / 简体中文版 2016 
- 个人分类：前端 / JavaScript
- ISBN：978-7-115-43116-5

## 书评

写于2023年1月29日。

和《On Java》那本书不同，这套书的上卷、中卷、下卷实际上是没什么关联性的，完全就是几本互不相干的书，所以书评也是分开来的。而《On Java》那本的基础卷和进阶卷是一本书，所以不分开来。

实话说这是一本还不错的书。正如副标题“Types & Grammar & Async & Performance”说的，这本书主要讲的是JavaScript中的类型、并发和性能。但比起上卷，这本书就要稍微令人失望一些了。

和上一本一样，本书实际上分为两部分，前半本讲类型及语法，后半部分讲异步及性能。

在我个人看来，前半本实在是乏善可陈。主要讲的类型在大多数JavaScript入门书中已经有比较详细的阐释了，只不过书中更多地讲述了一些细节，比如`==`的详细机制（虽然实际上无论在高程还是犀牛书中这部分都介绍得很细），各运算符的详细用法、转型等，个人认为对实际开发并无什么帮助，只能说或许对前端面试八股有点用吧。前半本共五章，四章类型，一章语法，实际上对语法的介绍也就是走马观花，毕竟JS的语法本身也没啥好讲的，没太大意思。说实话前半部分唯一让我记住的是作者比较有趣地提出了`~`运算符的奇特用法，即`~str1.indexOf(str2)`可以代替`str1.indexOf(str2) !== -1`作为条件判断，但这东西由于是经典的隐式转换，在TS里报错，所以实际上也没啥实用价值，更何况别人要是没看过这本书会不知道你写个`~`上去是什么意思。

整本书的核心我个人主要集中在后半本。后半本用两章作铺垫，讲述了异步的概念，和传统基于回调方式异步的弊端，然后在第三章引出并详细介绍了Promise的机理。这里对Promise的前世今生，存在价值及用法都讲得很好，值得一看。第四章讲了很多通过生成器和Promise并用编写类同步代码的方式，很有趣，但现在可能只是奇淫巧计了，因为async/await出现后就不再需要用生成器模拟协程了，但确实很有意思。第五章介绍了一些当时的性能优化方案，大多数方案现在都寄了，没啥用，只有其中提到的Web Worker留了下来，但API也改了不少。第六章讲了一些性能测试与调优有关的原则和技巧，我认为这部分写得还不错，是值得读的。

但后半本书我不知道是否是翻译的问题，有些地方比较晦涩，读起来不通顺。另外后半本书由于涉及到异步，本身也是比较烧脑的，需要多花点时间看懂。

所以整体上这本书就只有小半部分比较有价值，相比于上卷还是比较让人失望的。但这仍是比较值得看的一本书，如果上卷属于前端必读，那这本至少也是属于非常推荐的层次。当然，如果是不带脑子地看，还是不读为妙。作者书中有不少现在看来比较错误的见解，需要辩证地读，尽信书则不如无书嘛。
