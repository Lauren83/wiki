---
layout: post
title: D码点评:15 哪些语言特性有助于开发大型系统?
description: ~ 麻辣评点,善意满盈
author: zoomq
categories: gDgcoDe
tags:  gdg D码点评 dd wechat coding
---


# [@_李路 12月14日 23:43](http://weibo.com/1218520492/Anjfrp64i)
![131111_lilu.png(PNG 图像,428x371 像素)](http://pyconcn.qiniudn.com/images/speakers/131111_lilu.png?ver=20131211)

综合来说,java就是一门设计平庸,枯燥无味,为大公司所控制,官僚作风浓厚的语言,它主要用来指挥一大帮一点不喜欢编程的码农,去为一些大型组织完成某些大型任务,而这种任务的要求就是把愚蠢的人造成的伤害降低到最少. 而真正的程序员,需要的是语言强大的力量,来发挥,而不是限制自己的聪明才智. 

[PyCon2013China 珠海场](http://zhgdg.gitcafe.com/2013-12/et16-pycon-zh/)
讲师日前发布的一条 weibo 再次引爆了语言之争.

于是大妈想起了老庄的一篇神吐槽:

## [哪些语言特性,有助于开发大型系统](http://zhuanlan.zhihu.com/zhuangbiaowei/19598480)

来自: 知乎专栏 - 思考IT

<!--more-->


这个问题是我提的,主要的原因当然是因为自己也有所思考,想与各位朋友有所交流. 不过,这篇回答却拖了很多天,主要是腹稿没有打好的缘故. 

### 一,首先需要定义,何谓大型系统?

有一个答案是@jifei 写的,虽然他的答案被折叠了,但是我认为其实他提出的问题非常重要,必须首先解答. 

在我看来,在软件编程这个领域几十年的发展过程中,对于大型系统的定义,是一直在扩大着的. 最近我翻一本介绍编程语言的老书,说到当年 FORTRAN 语言刚刚面世的时候,尚且不能支持分别编译,导致程序超过400~500行,编译器就会死机. 那个时候的大型系统,也许就是超过500行代码的程序吧. 

随着软硬件各方面的发展,现在的程序已经远远超过这个规模了,按照@vczh 的定义,得超过8位数才行......

这就引出第二个需要讨论的问题,系统的大小,是由问题域的复杂度决定的?还是由解答域的复杂度决定的?

打个比方,如果在 UNIX 刚刚诞生的1969年,我们只有PDP-7这样的计算机,编程语言也只能选择 C 语言. 如果想要写一个知乎这样的网站,得花多少代码量呢?得付出多少的人力,物力呢?这样的一个网站,算不算大型系统呢?

假设一个系统,用 A 方法,A 语言实现,需要100万行代码;用 B 方法,B 语言实现,只需要10万行代码. 这个系统的算大型?算中型?还是算小型呢?

所以,在这里首先抛出两个观点:

    大型系统的定义,一直在不断增大
    大型系统的规模,取决于问题域,而非解答域

### 二,语言特性的目标
如果泛泛而谈,绝大多数的语言特性,在最初设计的时候,都是为了提高开发效率,简化开发劳动,从而帮助开发者开发更加大型的系统的. 

汇编替代机器码是如此,高级语言替代汇编也是如此. 举一个极端的例子:
最初的 FORTRAN 只允许 IJKLMN 六个变量作为循环中的变量. 据说大多数编程只需要用到IJK 三个,FORTRAN 的设计者已经大发慈悲,一口气给了六个了. 
到后来,变量名,函数名,方法名,类名都允许任意命名,任意长度,这就是一个巨大的进步,因为有意义的变量名,能够帮助写出有意义的代码. 
再到后来,ruby 有一个小小的改进,方法名中允许出现?号和!号,虽然只增加了一点点,但是也不无价值. 

### 三,早期的语言特性,大多数是为了方便程序员而设计的
早期的语言发展,可以说是在一片蛮荒之中,披荆斩棘地前进. 在没有浮点运算单元之前,只能模拟浮点运算,这是当年程序员的一大噩梦,但是到后来,这都不算一回事. 

函数定义,是为了能够少些重复的代码. 等到有高级语言,支持函数的递归调用以后,程序员就能够写更加简单和自然的代码了. 

绝大多数程序员,都最痛恨重复劳动,所以 DRY 原则是人人信奉的最高准则. 众多的语言特性,也为了更好的代码重用,而被设计出来. 比如模板,比如继承之类. 

### 四,意识到程序员需要被限制,是语言发展历程中的一大转折
程序员这个职业,经历了一个逐步走下神坛的过程. 最初的程序员,都是天才,都是神级的家伙,他们不会犯错,唯一限制他们的创造力的,是烂机器,烂工具与烂语言. 

渐渐的,程序员越来越多,那些不是天才的家伙,也混入了程序员的队伍. 天才们非常烦恼,却毫无办法. 

终于,有一些大神受不了了:[我要设计一种语言,让那些家伙去用,通过限制,让他们没法犯错!]

(以上为演绎,请勿对号入座)

Java 这样的语言,在历史上出现,并且广为流行,是有其必然性的. 虽然,其中的有些强制(比如 Exception),突显了语言设计者的傲慢与自以为是. 

### 五,类库与框架的出现,是一大进步
常年的劳动,使程序员们逐步的意识到,大型系统之间,是存在相似之处的,是可以归类的. 他们需要解决的问题,是可以逐步提炼出通用的解决方案的. 

最终,开发团队的工作分为两个阶段:挑选成熟的,适合系统需要的框架与类库,编写自己必须开发的代码. 

这时,对于语言特性的需求,就新增了对于框架与类库编写的支持能力. 

RTTI,反射,Interface,元编程,DSL 之类的技巧,被发展出来. 

插播,TDD 与单元测试思想的兴起
TDD 是个好东西,它从根本上分担了质量保证的责任,而不少语言,开始提供[assert]这样的关键字,也是一种语言层面的响应,个人认为是有进步意义的. 

### 六,开源时代与远程包管理
最为典型的例子是 ruby 的 gem 和 nodejs 的 npm,通过这两个工具,软件开发中自造轮子的现象大大减少,程序员们越来越习惯于首先搜索可能适用的 package,然后 net install 进来. 

这虽然不全然是语言特性,但确实是语言支持特性的最新的发展方向. 

仅仅比较 ruby 和 nodejs 来说,nodejs 的包管理比 ruby 更加完善合理,有兴趣的朋友,可以去了解一下. 

### 七,高负载,高并发带来的需求
这个值得专题讨论,此处不再赘述. 个人认为 Go 的出现,的确是针对这一类问题,有了更加深入的思考. 

### 八,结论

    语言特性,是一个历史发展的过程,最好从历史的角度来考察
    设计者的初衷往往都是好的,但是实际上有很多语言特性,事与愿违
    通过不断的分解,很多开发大型系统的困难,已经不再需要在语言层面解决
    编程语言仍然年轻,还在不断进步,值得不断的关注与学习


## 是也乎

[好吧](http://daily.zhihu.com/story/1657913)
, 这文章几乎是骂人不吐脏字儿的典范了...
[好吧](http://daily.zhihu.com/story/1657913)
, 虽然最后因为江湖的原因, 老庄打了手好太极,将场面话给说足了;
不过, 关键态度也已经表述明确了,
那就是: 程序员对于开发语言是有态度的, 不同的语言其发明/发展的使命是不同的.开发语言本身是否先进不是广告里说什么就是什么的...

大妈也崇敬了 JAVA 很多年, 曾经因为看不懂 Think in JAVA 以为自个儿没有程序员的素质...

但是,事实证明 [奧卡姆剃刀定律](http://wiki.mbalib.com/zh-tw/%E5%A5%A5%E5%8D%A1%E5%A7%86%E5%89%83%E5%88%80%E5%AE%9A%E5%BE%8B)
(Occam's Razor, Ockham's Razor)是靠谱的,
按照自个儿当下的积累, 42分钟里上不了手的,就不是适合你的,

但是,不代表这货不靠谱.

只是,说明当前强行使用之不是个事儿.

不过,不去尝试其它可能更加合用的 语言/框架/模块/库... 来解决当前的问题,
就认为自个儿会用的就是最好的,
那只能,呵呵呵了...




# 当期活动 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

## 12.21 CodeGirl.2

CodeGirl 是珠海GDG 原创品牌活动:

- 从讲师到参加者,都必须是 MM
- 程序猿一概不准进入,除非自个儿切了
- 营造出一个放松自在的分享氛围,成为本地 `程序媛` 的首选出没活动

[[12.21]专属女生的GDG珠海CodeGirl第二季来了,快来报名吧!](http://www.chinagdg.com/thread-3367-1-1.html)
,按时前往,享受纯纯的圣诞前...

我们已经成功组织了一期,记要在:Event:10 CodeGirls.1 Summary
      http://zhgdg.gitcafe.com/2013-10/et13-codegirl1-summary/


