## background图片不显示

问题环境：ios8/9

问题定位：在vue的template中，行内样式写入background-image，如果值使用了或，则部分老版本ios手机不显示图片


写法示例：

```
<div
  class="saler-avatar"
  :style="{'background-image': 'url(' + salerObj.avatar || defaultAvatar + ')'}"></div>
```
