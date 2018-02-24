---
title: 【译】13简单的优秀编码规则（从我15年的经验）
date: 2018-02-07 14:03:12
tags:
---

原文地址：https://hackernoon.com/few-simple-rules-for-good-coding-my-15-years-experience-96cb29d4acd9#.ddzpjb80c

![](http://p3alsaatj.bkt.clouddn.com/20180207140343_0UaL3X_Screenshot.jpeg)

嗨，我的工作作为一个程序员超过15年，并使用许多不同的语言，范例，框架和其他狗屎。我想和大家分享我写好代码的规则。

# 1. 优化VS可读性 去他妈的优化
始终编​​写易于阅读且对开发人员可理解的代码。因为在硬可读代码上花费的时间和资源将远远高于从优化中获得的。
如果你需要进行优化，那么使它像DI的独立模块，具有100％的测试覆盖率，并且不会被触及至少一年。

# 2. 架构第一
我看到很多人说“我们需要快速做事，我们没有时间做架构”。其中约99％的人因为这样的想法而遇到了大问题。
编写代码而不考虑其架构是没有用的，就像没有实现它们的计划一样，梦想你的愿望。
在编写代码的第一行之前，你应该明白它将要做什么，它将如何使用，模块，服务如何相互工作，它将有什么结构，如何进行测试和调试，以及如何更新。

# 3. 测试覆盖率
测试是好事，但他们并不总是负担得起，对项目有意义。

当你需要测试：
 - 当你编写模块时，微服务将不会被触及至少一个月。
 - 当你编写开源代码。
 - 当你编写涉及金融渠道的核心代码或代码。
 - 当您有代码更新的同时更新测试的资源。

当你不需要测试时：
 - 当你是一个创业。
 - 当你有小团队和代码更改是快速。
 - 当你编写的脚本，可以简单地通过他们的输出手动测试。

记住，`带有严格测试的代码可能比没有测试的代码更有害`。

# 4. 保持简单，极度简单
不要编写复杂的代码。更多更简单，那么更少的错误它可能有和更少的时间来调试它们。代码应该做的只是它需要没有非常多的抽象和其他OOP shit（尤其是涉及java开发人员）+ 20％的东西可能需要在将来以简单的方式更新它。

# 5. 注释
出现注释说明你的代码不够好。好的代码应该是可以理解的，没有一行注释。但是如何为新开发人员节省时间？ - 编写简单的内联文档描述什么和如何方法工作。这将节省很多时间来理解，甚至更多 - 它将给人们更多的机会来提出更好的实施这种方法。并且它将是全球代码文档的良好开端。

# 6. 硬耦合VS较小耦合
始终尝试使用微服务架构。单片软件可以比微服务软件运行得更快，但只能在一个服务器的上下文中运行。
微服务使您可以不仅在许多服务器上，而且有时甚至在一台机器上（我的意思是过程分发）高效地分发您的软件。

# 7. 代码审查
代码审查可以是好的，也以是坏的。
您可以组织代码审查，只有当您有开发人员了解95％的代码，谁可以监控所有更新，而不浪费很多时间。在其他情况下，这将是只是耗时，每个人都会讨厌这个。

在这部分有很多问题，所以更深入地描述这一点。

许多人认为代码审查是一个很好的方式教新手，或者工作在不同部分的代码的队友。但是代码审查的主要目标是保持代码质量，而不是教学。让我们想象你的团队制作代码用于控制核反应堆或太空火箭发动机的冷却系统。你在非常硬的逻辑中犯了巨大的错误，然后你给这个代码审查新的家伙。你怎么认为会发生意外的风险？ - 我的练习率超过70％。

良好的团队是每个人都有自己的角色，负责确切的工作。如果有人想要理解另一段代码，那么他去一个负责任去问他。你不可能知道一切，更好的优秀的理解小块代码而不是理解所有。

# 8. 重构没啥用
在我的职业生涯中，我听到很多次“不要担心，我们以后会重构它”。在未来，这会导致大的技术债务或从头开始删除所有的代码和写作。

所以，不要得到一个债务，除非你有钱从头开发你的软件几次。

# 9. 当你累了或在一个坏的心情不要写代码。

当开发人员厌倦时，他们正在制造2到5倍或者更多的bug。所以工作更多是非常糟糕的做法。这就是为什么越来越多的国家思考6小时工作日，其中一些已经有了。精神工作不同于使用你的二头肌。

# 10. 不要一次写全部 - 使开发迭代
在编写代码分析和预测之前，您的客户/客户真正需要什么，然后选择您可以在短期内以高质量开发的MVF（最有价值的功能）。使用这样的迭代来部署质量更新，而不是腰部时间和资源对不合理的愿望和牺牲与质量。

# 11. 自动化VS手动
自动化是长期的100％成功。所以如果你有资源自动化的东西，现在应该做。你可能认为“只需要5分钟，为什么我应该自动化？但让我计算这个。例如，它是5个开发人员的日常任务。 5分钟* 5天* 21天* 12个月= 6 300分钟= 105小时= 13.125天〜5250 $。
如果你有40 000名员工，这将需要多少费用？

# 12. 出去浪，学习新爱好
差异化工作可以增加心智能力，并提供新想法。所以，暂停现在的工作，出去呼吸一下新鲜空气，与朋友交谈，弹吉他等。
`ps: 莫春者，春服既成，冠者五六人，童子六七人，浴乎沂，风乎舞雩，咏而归。------《论语.先进》。`

![](http://p3alsaatj.bkt.clouddn.com/20180207140423_Iku4es_Screenshot.jpeg)


# 13. 在空闲时间学习新事物
`当人们停止学习时，他们开始退化。`