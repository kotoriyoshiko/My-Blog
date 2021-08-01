### Vue分为哪两个版本

1. 完整版 vue.js
2. 不完全版 vue.runtime.js

### 特点

1. 完整版含有compiler
2. 不完全版不含有compiler
3. 所以完整版体积要多于不完全版，compiler占40%体积

### 视图

1. 完整版可直接写在HTML里或者写在template里
2. 不完全版需要卸载render函数里用h来创建标签,(h是尤雨溪写好传给render的)

### 引入方法

1. cdn引入
2. webpack引入（默认使用的是不完全版，完整版需要配置alias）
3. @vue/cli引入 （默认使用的是不完全版,完整版需要去配置）

### 最佳实践

1. 总是使用非完整版,然后配合vue-loader和vue文件
2. 保证用户体验,用户下载的JS文件体积更小,但只支持h函数
3. 保证开发体验,开发者可直接在vue文件里写HTML标签,而不写h函数
4. 因为可以用vue-loader把vue文件里的HTML转换为h函数

codesandbox.io也可以创建vue项目
