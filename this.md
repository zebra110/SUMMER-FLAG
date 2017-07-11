### 1.new绑定?   this绑定的是新创建的对象
```
var bar = new foo();
```
绑定了bar

### 2.显示绑定 call/apply/bind(bind为es5中 把参数设置为this的上下文，并调用原始函数) 硬绑定？ this绑定的是指定的对象
```
var bar = foo.call(obj2);
```
绑定了obj2

###3.隐式绑定 某个上下文对象 this绑定那个上下文对象
```
var bar = obj.foo();
```
绑定了obj

###4.默认绑定
```
var bar = foo();
```
绑定了window
