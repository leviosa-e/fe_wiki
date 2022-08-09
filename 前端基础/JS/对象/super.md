# super

`super` 关键字用于访问和调用一个对象的**父对象**上的函数。

## 语法

```js
super([arguments]);
// 调用 父对象/父类 的构造函数

super.functionOnParent([arguments]);
// 调用 父对象/父类 上的方法
```

## 描述

在构造函数中使用时，super 关键字将单独出现，并且**必须在使用 this 关键字之前使用**。  
super 关键字也可以用来调用父对象上的函数。

## 示例

### 1. 删除 super 上的属性将抛出异常

不能使用 `delete` 操作符 加 super.prop 或者 super[expr] 去删除父类的属性，这样做会抛出 ReferenceError。

### 2. 在对象字面量中使用 super.prop

```js
var obj1 = {
  method1() {
    console.log("method 1");
  }
}

var obj2 = {
  method2() {
   super.method1();
  }
}

Object.setPrototypeOf(obj2, obj1);
obj2.method2(); // logs "method 1"
```