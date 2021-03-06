# 设计稿及尺寸单位

结合过往的开发经验，Taro 默认以 `750px` 作为换算尺寸标准，当设计稿宽度为 `750px` 时，在 Taro 中书写尺寸按照 1:1 的关系来进行书写，即从设计稿上量的长度 `100px`，那么尺寸书写就是 `100px`，当转成微信小程序的时候，尺寸将默认转换为 `100rpx`，当转成H5时将默认转换为以 `rem` 为单位的值。

如果设计稿不是以 `750px` 为标准，则需要在项目配置 `config/index.js` 中进行设置，例如设计稿尺寸是 `640px`，则需要修改项目配置 `config/index.js` 中的 `designWidth` 配置为 `640`：

```javascript
const config = {
  projectName: 'myProject',
  date: '2018-4-18',
  designWidth: 640,
  ....
}
```

建议使用 Taro 时，设计稿以 iPhone6 `750px` 作为设计尺寸标准。
