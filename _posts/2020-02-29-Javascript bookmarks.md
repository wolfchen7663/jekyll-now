## 记录学习 JavaScript 的一些要点

### 字符串

字符串的输出最好使用这样的格式(模板字面量格式):
```
`${a}bbb${c}`
```
**字符串标签模板:**

![字符串标签模板](https://github.com/wolfchen7663/wolfchen7663.github.io/blob/master/_posts/%E5%AD%97%E7%AC%A6%E4%B8%B2%E6%A0%87%E7%AD%BE%E6%A8%A1%E6%9D%BF.png?raw=true)


字符串的截取
```
// 遵循左闭右开的原则
str.slice(1, 4) 
str.substring(1, 4)
str.substr(1, count) //count 表示截取的个数

str.slice(-3, -1)
str.substring(-3, -1) // 为空
str.substring(-3) // 还是原字符串，这就表明这个对负数不敏感
str.substr(-3, 2) 2 表示截取俩个
```

字符串的替换
`str.replace(“被替换的","新的")`


Boolean
数值类型和字符串类型`0 和 "" 是 false`
引用类型`[] 和 {} 是 true`


数组的填充
`array.fill("something", 1, 4)`
左闭右开

数组的截取
`array.slice(1, 4)` 左闭右开进行截取，注意不改变原数组
`array.splice(1, 4)` 左闭，**右边是截取几个，注意这个时候会改变原数组。相当于删除数组里面的元素**

用`splice`进行数组元素的替换
`array.splice(1, 1, "add")`将第二个元素替换为"add"

用`splice`进行数组元素的增加
`array.splice(1, 0, "add")`，在第二个位置添加"add"




