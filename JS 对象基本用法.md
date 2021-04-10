## 声明对象的两种语法

1. let obj = {'name':'frank', 'age':18}    //name就是键 frank就是值  在一起就是键值对
2. let obj = new Object({'name':'frank'}) //这是正规写法但是没必要这么写,用上面的就行
3. console.log({'name':'frank','age':18}) 

## 删除对象属性

1. delete obj.xxx     
2. delete obj['xxx']    //即可删除obj的xxx属性

## 查看对象属性

### 查看全部属性
1. Object.keys(obj)  //查看对象所有属性
2. Object.values(obj)   //查看对象所有值
3. Object.entries(obj)  //查看所有属性和值 

### 查看单个属性

1. 中括号语法：obj['key']
2. 点语法：obj.key
3. 坑新人语法：obj[key] //变量key值一般不为‘key’
4. 优先使用中括号语法

## 修改或增加对象属性

1. let obj={name:'frank'}  //name是字符串
2. obj.name='frank'  //name是字符串
3. obj['name']='frank'      //注:obj[name]='frank' 是错的,因为name值不确定
4. obj['na'+'me']='frank'
5. let key='name';  obj[key]='frank'  //obj.key='frank'是错的. 等价于obj['key']
6. Object.assign(obj, {age:18, gender:'man'}) //批量赋值

### 'name' in obj和obj.hasOwnProperty('name') 的区别

1.'name' in obj无法区分是自己有的属性还是共有属性
2. obj.hasOwnProperty('name')就只能看自己的
