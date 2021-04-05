## 浏览器渲染原理

### 浏览器渲染的步骤

1. 根据HTML构建HTML树(DOM)
2. 根据CSS构建CSS树(CSSOM)
3. 将两棵树合并成一颗渲染树(Reader tree)
4. Layout 布局(文档流，盒模型，计算大小和位置)
5. Paint 绘制(把边框颜色，文字颜色，阴影绘制出来)
6. Composite 合成(根据层叠关系展示画面)

### 三种更新方式

1. 全部执行渲染步骤 //例如：div.remove会触发当前元素消失,其他元素重新布局
2. 跳过layout，直接repaint和composite  //例如：改变背景颜色
3. 跳过layout和paint,直接composite //例如：改变transfrom

### 其他

1. https://csstriggers.com/ 可查询不同属性会触发什么流程


## CSS动画的两种做法

### transition

#### transition作用:补充中间帧

#### 语法

1. transition:属性名 时长 过渡方式 延迟   //例:transition:left 200ms linear
2. 可以用,分隔两个不同属性 //例:transition:left 200ms,top 200ms
3. 可以用all代表所有属性 //例:transition:all 200ms
4. 常用过渡方式: linear/ease/ease-in/ease-out

#### 注意

1. 不是所有属性都能过度 例:display:none=>black无法过度
2. 一般改成visibility:hidden=>visible(不要问为什么)
3. 在transition取值后加上forwords可以让动画停在最后一帧

### animation

#### animation用法

1. 生命关键帧@keyframes
2. 添加动画animation

#### @keyframes写法

1. 搜索 keyframes mdn
2. 一种写法是用 from to //动画的两个状态 开始和结束
3. 百分数表示 //不同时间点 动画的样式 

#### animation缩写语法

animation:时长/过渡方式/延迟/次数/方向/填充模式/是否暂停/动画名








