# JavaScript code point

## 將數字變成字元

```js
String.fromCharCode(65); // "A"

"A".charCodeAt(0); // 65

str = "0x6211";
//"0x6211"
parseInt(str, 16);
//25105
num = 0x6211;
//25105
num.toString(16);
//"6211"
```

## Number to String

```js
chtCode = 24859;
chtCode.toString(2);
//"110000100011011"
chtCode.toString(16);
//"611b"
```

## String to Number

```js
str = "110000100011011";
parseInt(str, 2);
//24859
str = "611b";
parseInt(str, 16);
//24859
0x611b;
//24859
```

```js
let str = "我愛你";
for (i = 0; i < str.length; i++) {
  console.log(
    i,
    str.charCodeAt(i),
    str.charCodeAt(i).toString(16),
    String.fromCharCode(str.charCodeAt(i))
  );
}
// 0 25105 "6211" "我"
// 1 24859 "611b" "愛"
// 2 20320 "4f60" "你"
```

## ES6

U+0041 (0041 代表 Code Point 編碼位置)

```js
"ABC".codePointAt(0);
//65
String.fromCodePoint(0x0041, 0x0042, 0x0043);
//"ABC"
let x = "\u0041\u0042\u0043";
//"ABC"
```
