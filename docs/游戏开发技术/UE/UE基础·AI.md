# UE基础·AI

本文主要介绍虚幻引擎中AI相关的基础知识。

在虚幻中一般使用AIController来控制玩家以外的NPC角色，其中还会涉及到虚幻的行为树、黑板和EQS等内容，这篇文章会简要介绍它们的概念和使用方法，并在文章末尾附上更加深入的文章推荐，方便想要了解其具体原理的同学参考

本文介绍的内容为以下几个：

- AIController
- 行为树
- 黑板
- AI Perception
- EQS
--插一张图片--

## AI 控制器（AI Controller）

AIController是专门用于控制Pawn/Character的特殊Controller，是控制NPC角色的灵魂。一般会在Pawn/Character中编写角色的能力和属性，在AIController中决定怎么使用这些能力。

AIController可以和行为树、黑板、AIPerception等模块进行交互，并实现它们之间通信的方式，你可以把它看作一个管理者，不同的模块实现不同的功能，它负责在中间统筹调度，进而控制角色的行为

在这些模块中：
**行为树** 是AI的决策工具
**黑板** 是AI的数据储存容器
**AIPerception** 实现AI的感知能力
**EQS** 实现AI的环境查询能力


## 行为树（Behavior Tree）

行为树是一种可视化的AI决策工具，通过树型结构定义AI的决策逻辑

整个行为树有很多个节点组成，有以下几个节点类型：
- **选择器Selector**
- **序列Sequence**
- **平行节点Parallel**
- **任务Task**
- **装饰器Decorator**
- **服务 Service**
  


## 黑板（Blackboard）

黑板用于存储AI运行时需要的数据。行为树节点可以读取和写入黑板上的数据，实现信息共享。也可以通过setblackboardvalue在AIController中改变黑板的值

## AIPercepton

AI的感知系统，集成在AIPerception组件上，组件内置了视觉，听觉，触觉等基本感官，并且可以为单独的感官设置不同的参数实现不同的感知效果。

## 环境查询系统（EQS）

EQS是一个环境查询系统，AI可以使用它在环境中筛选最优点，比如说用来查找最近的掩体或者找到最佳的攻击位置
