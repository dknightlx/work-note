## 运算优先级导致background图片不显示

问题环境：ios 10.1.1

问题定位：vue的template中，字符串拼写要注意运算符的优先级问题


写法示例：

```
<div
  class="saler-avatar"
  :style="{'background-image': 'url(' + avatar || defaultAvatar + ')'}"></div>
```

正确写法：或运算应该首先执行

```
<div
  class="saler-avatar"
  :style="{'background-image': 'url(' + (avatar || defaultAvatar) + ')'}"></div>
```
