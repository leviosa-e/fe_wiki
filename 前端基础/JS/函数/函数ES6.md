# 函数ES6

## rest 参数

### 1. arguments 对象与 rest 参数

* arguments 对象是类似数组的对象，有 length 属性，但是无法使用数组方法，需要先使用 Array.from(arguments) 转换为数组

* rest 参数就是一个数组，可以使用数组方法

```js
// arguments 写法
function sortNumber() {
  return Array.from(arguments).sort()
}

// ...rest 写法
function sortNumbers(...nums) {
  return nums.sort()
}
```

### 2. rest 参数只能放在最后，否则会报错

### 3. 函数的 length 属性不包括 rest 参数