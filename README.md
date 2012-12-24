# animate.css

---

Css 3 动画样式。

---


## 使用说明

[官方教程](https://github.com/daneden/animate.css)

引入样式文件，绑定对应的 className。

```js
seajs.use(['$', 'alice/animate/1.0.0/animate.css'], function($) {
    $('#test').addClass('animated bounceOutLeft');
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

[所有 className](http://daneden.me/animate/)

