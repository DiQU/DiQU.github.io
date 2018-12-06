```js
let a='b'
x={
	a:'a',
	func:function(){console.log(this.a)}
}
//{a: "a", func: ƒ}
y={
	a:'a',
	func:()=>{console.log(a)}
}
//{a: "a", func: ƒ}

x.func()
//a
y.func()
//b

x.func.apply()
// b
```