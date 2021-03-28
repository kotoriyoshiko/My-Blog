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
