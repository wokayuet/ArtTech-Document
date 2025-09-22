# UE进阶

初步熟悉了蓝图和C++之后，可以着手开始对UE多个模块的深入学习，本文主要参考[这篇文章](https://zhuanlan.zhihu.com/p/659805638),简要介绍UE中的各个模块并给出相应的教程供大家学习。

学习的过程中可以根据自己的需要有目的性的去搜索对应的内容，如果下面的教程不太适合你可以拿着相应的关键词去查找，有疑惑的地方可以询问AI。

## 编程
这一模块的内容主要是帮助大家更加深入的了解虚幻的蓝图和C++编程方面的内容，对实际的开发作用很大。
[UE5标识符详解 | 史上最全](https://zhuanlan.zhihu.com/p/717920216)
[InsideUE4:UObject](https://zhuanlan.zhihu.com/p/24319968)
[深入蓝图开发：理解蓝图技术架构](https://neil3d.github.io/unreal/bp_in_depth.html)
[官方文档：用C++编程](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/programming-with-cplusplus-in-unreal-engine) && [官方文档：蓝图](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/blueprints-visual-scripting-in-unreal-engine)
书籍：**《大象无形：虚幻引擎程序设计浅析》**

## AI
虚幻的AI使用的是内置的行为树和AIPerception等内容，你可能已经初步掌握了它们的使用方法，这一部分的内容就帮助你去了解它们的底层原理，把握具体的逻辑。
[AI行为树系统源码解析](https://zhuanlan.zhihu.com/p/368889019)
[AIPerception部分源码讲解](https://supervj.top/2023/02/01/AI_Percenption/) && [深入理解AI感知系统](https://blog.csdn.net/hacning/article/details/142262772) && [自定义AI感知](https://blog.csdn.net/hacning/article/details/142262772)
[Navmesh底层原理](https://zhuanlan.zhihu.com/p/74537236) && [Navmesh源码剖析](https://zhuanlan.zhihu.com/p/691181077)
[官方文档：AI](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/artificial-intelligence-in-unreal-engine)

## 动画
先对虚幻内置的动画系统学习之后，可以去学习ALS高级运动系统和lyra项目的动画实现，ALS是UE的一个插件，它实现了3A级别的移动动画，还具有动画相关的多种功能。lyra项目则是虚幻引擎推出的初学者项目（实际上整个项目的难度级别并不是初学者水平），其中动画实现运用了UE5新的动画技术，和ALS相比各有优劣，大家可以选择性学习。
[解析UE动画系统](https://segmentfault.com/a/1190000044591404#item-2) && [UE4/UE5 动画的原理和性能优化](https://zhuanlan.zhihu.com/p/545596818)
[Lyra vs ALS](http://www.lpq.design/2024/04/LyraVsALS/)
[Lyra的动画蓝图](https://zhuanlan.zhihu.com/p/517368184)
[深入浅出学习ALS高级运动系统视频教程](https://www.bilibili.com/video/BV12f4y1r71N/?p=2&vd_source=dba8b21354c8531d018170bccdb5ad3a)
[官方文档：动画](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/animating-characters-and-objects-in-unreal-engine)

## UI
主要学习UMG和Slate，UMG是蓝图层级的UI框架，提供了很多现成的控件，比如按钮进度条这种，可以在Widget蓝图上拖拽制作UI并编写交互逻辑，上手快和直观。Slate则是C++层级UI框架，可以用来定制化控件，会比直接用UMG麻烦点。
[参考文章](https://zhuanlan.zhihu.com/p/659805638)UI部分内容，学习各个控件的使用细节
[UMG生命周期](https://www.cnblogs.com/sin998/p/15490311.html)
[UE5Slate基础](https://zhuanlan.zhihu.com/p/636153935)

## Gameplay框架
这一部分是学习UE的玩法框架，首先了解虚幻的整个GamePlay架构，然后需要学习虚幻的技能系统即GAS，GAS可以帮你实现一整套复杂的技能系统，同时易于配置和扩展，UE5还提供了GameFeatures架构，这个架构是用来扩充玩法的，你可以将一套玩法做进一个GameFeatures模块里，用的时候就跟插件一样即插即用。
[InsideUE4:GamePlay架构](https://zhuanlan.zhihu.com/p/22833151)
[GAS入门(视频)](https://www.bilibili.com/video/BV1X5411V7jh/) && [GAS各个模块的介绍及使用](https://zhuanlan.zhihu.com/p/486808688) && [官方文档：GAS](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/gameplay-ability-system-for-unreal-engine)
[InsideUE5: GameFeatures](https://zhuanlan.zhihu.com/p/467236675)


## 网络
这一部分需要研究UE自己的网络架构以及网络复制等相关内容
[官方文档：网络](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/networking-overview-for-unreal-engine)
[UE网络同步](https://zhuanlan.zhihu.com/p/719982909)
[网络同步原理深入](https://zhuanlan.zhihu.com/p/34723199)