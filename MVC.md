### MVC三个对象分别做什么

1. M-Model(数据模型)负责操作所有数据
2. V-View（视图）负责所有UI界面
3. C-Controller(控制器)负责其他

### EventBus 有哪些 API，是做什么用的

1. eventBus 可以满足最小知识原则，m 和 v 互相不知道对方的细节，但是却可以调用对方的功能,主要用于对象间通信
2. eventBus 提供了 on、off 和 trigger 等 API，on 用于监听事件，trigger 用域触发事件
