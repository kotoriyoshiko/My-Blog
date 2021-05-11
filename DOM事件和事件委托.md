#### DOM事件
从外向内找监听函数,叫事件捕获

从内向外找监听函数,叫事件冒泡

### 事件绑定API
````
IE：id.attachEvent('onclick',fn) //冒泡
网景： id.addEventListener('click',fn) //捕获
W3C：id.addEventListener('click',fn,bool) // bool不传值或价值默认走冒泡,传值为true走捕获
````
### W3C事件模型

先捕获(先爸爸=>儿子) 再冒泡(再儿子=>爸爸)

#### 事件委托

其实就是监听父元素或祖先元素

###优点

1. 减少内存消耗
2. 动态绑定事件




