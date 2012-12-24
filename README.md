# animate.css

---

Css 3 动画样式。

---


## 使用说明

[官方教程](https://github.com/daneden/animate.css)

单独打包引用或通过 seajs.use 引入样式文件，然后绑定对应的 className。

```js
seajs.use(['$', 'alice/animate/1.0.0/animate.css'], function($) {
    $('#test').addClass('animated bounceOutLeft');  // bounceOutLeft 可替换成你想要的效果
});
```

改变动画元素的动画参数。

```css
#yourElement {
    -vendor-animation-duration: 3s;
    -vendor-animation-delay: 2s;
    -vendor-animation-iteration-count: infinite;
}
```

## API

[所有 className 在此](http://daneden.me/animate/)

