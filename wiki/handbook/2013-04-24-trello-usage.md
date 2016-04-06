# Trello使用手册

[TOC]


感谢 上海GDG 如此郑重的邀请俺来作Trello 观察员,分享以往进行过程改进后遇到Trello 的直觉使用体验:

## 准备知识

- [硝烟中的Scrum和XP](http://www.infoq.com/cn/minibooks/scrum-xp-from-the-trenches)
    - [看板和Scrum--相得益彰](http://www.infoq.com/cn/minibooks/kanban-scrum-minibook-cn)
    - [5W1H](http://wiki.woodpecker.org.cn/moin/5W1H)
    - [SMART原则 - MBA智库百科](http://wiki.mbalib.com/wiki/SMART%E5%8E%9F%E5%88%99)
- 如果没有项目管理经验,以及敏捷开发的体验,使用Trello 绝对是摸不到头脑的
- 因为 Trello 的主创者是Joel 哪!
    - 就是那个通过自个儿的Blog 吸引到一大批NB 的人,给自个儿开发自个儿用的爽的系统,而且赚钱了的Joel !
    - [软件随想录 : 程序员部落酋长Joel谈软件](http://book.douban.com/subject/4163938/)
    - [Joel说软件 : Joel on Software](http://book.douban.com/subject/1426838/)

<!--more-->

## 协同原则

- 共识为先
    - Trello 是为了解决小团队内部复杂事务协同的
    - 所以,怎么使用Trello 一定要参与的全员都认可所有原则,才可能用起来!
    - 以俺在多种团队中使用的体验总结,至少应有以下原则被事先承认:
        - 只要被认领/指派的 card 就一定要有个结果
        - card 的 DONE 一定要有成员核查过,不能自说自话的移动过去
        - 每个成员,同一时刻在 DOING 的card 不应该超过2个!
- 严格执行
    - 有了团队共同规约后,一定要严格执行,在有协同
    - 否则,只有其中一两位成员在每天使用 Trello ,其它成员从来不打开来更新,没P 用的!
    - 所以,Trello 只是工具,不是管理制度
    - 制度的执行,要社区其它管理行为加以保证
    - 要尽可能的通过任何可能的渠道强调 Trello 是社区正式事务的唯一执行评证,才可能让大家在使用中喜欢上 Trello 吧...
- 随时改进
    - Trello 基于 Joel 多年的敏捷开发管理经验,是Scrum 式过程的最小集合!只提供了最最最 基本的看板功能...
    - 所以,每个项目都有自个儿不同的领域问题,一定要根据大家使用中的问题,及时调整使用规约,让大家感觉到 Trello 是自个儿的工具,越用越爽才能真正发挥作用!


## 直觉使用
Trello 其实就是对现实即时贴形成的Kanban 系统的在线模拟,所以,其使用可以完全根据现实 Kanban 的使用来!

### 固定流动方向

所有任务卡的生命周期一致:

- INBOX 中自由创建,收集需求
- TODO 中主动认领,完成任务分配
    - 简单的进入 card 按空格,就将自个儿的头像缀入card 表示这活儿俺作了!
    - 也可以通过 Assign 指派某个成员为当前 card 的执行人
- DOING 中宣告执行状态
    - 注意,DOING 泳道中任何时刻,存在的card 不应该超过成员总数的2倍
    - 因为每个人,同时不应该作两件以上的事儿!
- CHECKING 中进行review 确保任务完成了预设目标
    - 等同于软件开发中的 code review 过程
    - 大家可以主动评审,也可以约定固定的主持人来复查
    - review 人一定要留下评注,以便明确职责
- DONE 暂存当前阶段完成的事务
    - 每次活动真正完成后,应该都进行归档,重新开始
    - 当然,发觉有任务是相似出现的,应该进行 card 的复制,重新一轮

### 任务的SMART 设立

类似列表中提问邮件,要吻合 "[提问的智慧](http://wiki.woodpecker.org.cn/moin/AskForHelp)"原则;
任务卡的内容,也应该吻合管理学中的[SMART原则](http://wiki.mbalib.com/wiki/SMART%E5%8E%9F%E5%88%99)

- 可完成
    - 立个类似世界和平的任务卡当然是没有人去执行的
    - 任务应该足够明确,颗粒适当,就GDG 而言,是 `一个志愿者可以在1周以内完成的!`
- 可衡量
    - 怎么是作完了,怎么算作的好?
    - 一定要有个可以帮助成员判定自个儿是否作完的判定指标
    - 无法进行衡量的任务是不可能的任务,分配下去是坑人!
- 可执行
    - 不能假设所有志愿者都是经验人士
    - card 中应该尽可能的给出具体的执行指导,以便成员可以参考,也帮助理解任务的真正目的
- 有关联
    - Trello 之所以存在就是因为一个组织里,任何一个任务都不是单独存在的
    - 所以,card 中大可以加入其它card 的链接,说明当前任务的上下文,以便成员 DOING 时,以正确的顺序来完成
    - 比如,易拉宝的完成,就可以设立为:
        - 易拉宝设计
        - 易拉宝制作
        - 易拉宝部署
        - 易拉宝回收
        - 以上几个独立的SMART 任务卡进行关联性追踪
- 有边界
    - 所有活动/项目,时间/资金/人力,都是受限的!
    - 所以,在 card 中指明关键资源限制非常必要!
    - Trello 提价了 Due date ~ 截止时间设定,请使用!


### card 的执行中增补

Trello 最爽利的功能之一就是支持Markdown 格式! 所以,应该多多使用!

- 在任务的描述中尽可能详尽的说明SAMRT
- 而执行过程中,应该要求成员,将所有执行的证据链接/文档,进行增补
    - 将 card 视作维基文章进行增补
    - card 中的 checklist 只是个执行的要点提醒
    - 具体每个要点的执行成果,应该以链接或是附件的形式记录在card 中!
- 这样形成几个最佳体验:
    - 每个card 都产生了新的可用资源,比如文档/设计图形,保存在Trello 中,以后随时复用
    - 每个card 其实自然形成了活动总结中的一个章节,进行会后总结时,直接复制过去就好
    - 嗯嗯嗯,前提是社区的blog 是支持 Markdown 的
        - 当然现在这完全是可行的 ;-)
        - 个人推荐 gircafe 的 pages 服务
        - 比如:[ZHGDG Blogging](http://zhgdg.gitcafe.com/)


## 针对GDG 事务的建议

- 关键信息维基
    - 除了追踪任务,其实Trello 也可以作为内部维基
    - 将重要讲师/资源/主机SCM 信息...
    - 记述下来,因为 Trello 内置非常完善的全文搜索
    - 所以,当成社区维基完全可以!
- 核心事务协同
    - 这是Trello 的本意
    - 也是所有社区最应该积极合理使用的方式
    - 将一个活动各种事务,放在专用板中,可以宏观的掌握整体进展
    - 只是,这就要求,每个 Board 应该是:
        - 明确的
        - 受限的
        - 可用的
    - 即,任务板应该是同明确的活动相关的,不能什么活动都堆在一齐,大家用起来就容易混乱
        - 这也是维基的文化,每个维基应该只关注一种事物!
    - 太多card/成员,挤在一个 board 中,是无法协同起来的,沟通成果高过执行成本时,就没人用了
        - Trello 使用Kanban 的形式,将沟通成本尽可能的降低
        - 但是,一个专用board 中的成员超过7人,也将快速腐化
    - 可用其实才是根本,而可用的基础就是所有成员,达成共识,都能认同流程, `主动` 按规约推动每个card 的前进
- 移动提醒板
    - Trello 之所以,被这么多团队使用,其实最大的好处是全平台兼容的!
    - 我们可以使用 移动应用的 Trello 在现场/在室外,随时查阅信息,更动执行,关注提醒...
    

## 小技巧

- checklist 是可以复用的
    - 如果发现活动相关环节,每次组织时,都会发生
    - 那么一个完备的checklist 可以随时从上次 card 中复制过来
