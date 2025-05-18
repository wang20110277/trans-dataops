# trans-dataops
Easy Extract,Quick Transform,Limitless Load, This is DataOps ToolKits

不同的数据源头被抽象成不同的Reader插件，不同的数据目标被抽象成不同的Writer插件。理论上，FlinkX框架可以支持任意数据源类型的数据同步工作。作为一套生态系统，每接入一套新数据源该新加入的数据源即可实现和现有的数据源互通。

在底层实现上，FlinkX依赖Flink，数据同步任务会被翻译成StreamGraph在Flink上执行，基本原理如下图：
