### MVC三个对象分别做什么

1. M-Model(数据模型)负责操作所有数据
2. V-View（视图）负责所有UI界面
3. C-Controller(控制器)负责其他

````
const m = {
  data: {
    n: parseInt(localStorage.getItem("n")),
    }
}; //存数据

const v = {
  html: `
    <div>
        <div class="output">
          <span id="number">{{n}}</span>
        </div>
        <div class="actions">
          <button id="add1">+1</button>
          <button id="minus1">-1</button>
          <button id="mul2">*2</button>
          <button id="divide2">÷2</button>
        </div>
      </div>
`   //存视图

const c = {
      //存其他内容
      }
````



### EventBus 有哪些 API，是做什么用的

1. eventBus 可以满足最小知识原则，m 和 v 互相不知道对方的细节，但是却可以调用对方的功能,主要用于对象间通信
2. eventBus 提供了 on、off 和 trigger 等 API，on 用于监听事件，trigger 用域触发事件

````
const eventBus = $({}); //声明eventBus

const m = {
  update(data) {
    Object.assign(m.data, data);
    eventBus.trigger("m:updated");   //触发eventbus的m：updated事件
    localStorage.setItem("n", m.data.n);
  },
};
const c = {
eventBus.on("m:updated", () => {  //监听m:updated事件
      v.render(m.data.n);
})
}
````


### 表驱动编程是做什么的

1. 表指的是哈希表
2. 表驱动编程可以减少重复代码，只讲重要的信息放在表里，然后利用表来编程

### 如何理解模块化

1.现在完全理解不了,把简单的代码写那么复杂,咋理解？
