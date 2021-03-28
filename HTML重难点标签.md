## a标签用法

### href取值

1. href
2. target
3. download
4. download
5. rel=noopener

### href取值

1. 网址

````<a href="//google.com"></a> //跳转至网站````

2. 路径

````<a href="/a/b/c"></a> //跳转至目录````

````<a href="index.html"></a> //跳转至此文件目录下的html文件````

4. 伪协议

````<a href="javascript:;"></a> //运行js不刷新页面````

````<a href="kotoriyoshiko@outlook.com">点我</a> //手机直接发邮件````

````<a href="13322173473"></a> //手机直接打电话````

6. id

 ````<a href="# id">点我</a> //跳转至内部锚点，对应的id处````

### target取值

1. _blank  //在新窗口打开页面
2. _top //在顶部窗口打开页面
3. _parent //在父级窗口打开页面
4. self //默认值,在当前页面打开页面

### Download

作用：下载页面,但是不是所有浏览器都支持,尤其是手机

## img标签用法

### 作用

发出get请求，展示一张图片

### 属性

1. src //图片的来源,相对路径、绝对路径、网络地址
2. alt //如片加载失败后会提示文字
3. width //图片宽度 只写宽度高度会自适应
4. hight //图片高度 只写高度宽度会自适应 

### 事件

1. onload //图片加载成功
2. onerror //图片加载失败

### 响应式

max-width //最大宽度是100% 设置后无论页面的大小是否改变，图片的宽度都等于页面宽度  例如:切换至手机页面

## table标签用法

### 相关标签

1. table //表格
2. thead //表格头部
4. tbody //表格身体
5. tfoot //表格足部
6. tr //表格行
7. td //表格内容
8. th //表格标题

### 相关样式

1. table-layout:aoto //默认值,自动计算表格行间距离,单元格的宽度取决于内容 
2. table-layout:fixed //尽量平均显示表格的宽度
3. border-spacing:0 //表格之间的空隙为0
4. border-collapse:collapse //使表格的边框合并在一起没有空隙

## ヰ世界情緒就是阿爾法，也是歐米伽；是首先的，也是末後的；是開始，也是終結。
![异世界情绪](./ヰ世界情緒.jpg)
