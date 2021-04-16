## JS函数的执行时机

例1:console.log(a)什么都没有打印,因为根本没有调用！
```
let a = 0
function fn(){
  console.log(a)
  }
```

例2:打印出2,因为调用函数时,a的值已经是2
```
let a = 0
function fn(){
  console.log(a)
  }
a=2
fn()
```

例3:打印出6个6,因为先执行for循环后的值是6,i只有一个值,然后再打印的6次,所以是6个6
```
let i = 0
for(i = 0; i<6; i++){
  setTimeout(()=>{
    console.log(i)
  },0)
}
```

例4:打印出0，1，2，3，4，5,因为i会分别等于0,1,2,3,4,5,每个值打印一次,所以是6个值
```
for(let i = 0; i<6; i++){
  setTimeout(()=>{
    console.log(i)
  },0)
}
```
