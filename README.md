# animate.css

---

Css 3 动画样式。

---


## 使用说明

[官方教程](https://github.com/daneden/animate.css)

通过 link 打包引用或使用 seajs.use 引入样式文件，然后绑定对应的 className。

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


## 演示

> 以下动画效果在支持css3 animate的高级浏览器中有效。


<style>
.animate-obj {
    width: 80px;
    height: 80px;
    background-color: #42B8F7;
}
</style>

<div id="test1" class="animate-obj"></div>
<button id="trigger1">点击触发动画</button>

````js
seajs.use(['$', './src/animate.css'], function($) {
    $('#trigger1').click(function() {
        $('#test1').addClass('animated bounceOutLeft');
    });
});
````

<div id="test2" class="animate-obj"></div>
<button id="trigger2">点击触发动画</button>

````js
seajs.use(['$', './src/animate.css'], function($) {
    $('#trigger2').toggle(function() {
        $('#test2').addClass('animated');
        $('#test2').removeClass('fadeOutRightBig').addClass('fadeInRightBig')
    }, function() {
        $('#test2').removeClass('fadeInRightBig').addClass('fadeOutRightBig');
    });
});
````

<div id="test3" class="animate-obj"></div>
<button id="trigger3">点击触发动画</button>

````js
seajs.use(['$', './src/animate.css'], function($) {
    $('#trigger3').click(function() {
        $('#test3').addClass('animated rotateInUpRight');
    });
});
````

