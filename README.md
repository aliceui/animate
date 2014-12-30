# animate.css

---

Css 3 动画样式。代码来自：https://github.com/daneden/animate.css

---


## 使用说明

[官方教程](https://github.com/daneden/animate.css)

通过 link 打包引用或使用 seajs.use 引入样式文件，然后绑定对应的 className。

```js
seajs.use(['jquery', 'alice/animate/1.0.0/animate.css'], function($) {
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
    display: inline-block;
    padding: 0 20px;
    height: 60px;
    background-color: #112233;
    border-radius: 6px;
    opacity: 0.9;
    color: #fff;
    line-height: 60px;
    text-align: center;
}
</style>

<div id="test1" class="animate-obj">bounceIn</div>
<button id="trigger1">点击触发动画 bounceIn</button>

````js
seajs.use(['jquery', 'index.css'], function($) {
    $('#trigger1').click(function() {
        $('#test1').addClass('animated bounceIn');
    });
});
````

<div id="test2" class="animate-obj">fadeInUp</div>
<button id="trigger2">点击触发动画 fadeOutRightBig</button>

````js
seajs.use(['jquery', 'index.css'], function($) {
    $('#trigger2').click(function() {
        $('#test2').addClass('animated fadeInUp');
    });
});
````

<div id="test3" class="animate-obj">rotateInUpRight</div>
<button id="trigger3">点击触发动画 rotateInUpRight</button>

````js
seajs.use(['jquery', 'index.css'], function($) {
    $('#trigger3').click(function() {
        $('#test3').addClass('animated rotateInUpRight');
    });
});
````

<div id="test4" class="animate-obj">tada</div>
<button id="trigger4">点击触发动画 tada</button>

````js
seajs.use(['jquery', 'index.css'], function($) {
    $('#trigger4').click(function() {
        $('#test4').addClass('animated tada');
    });
});
````

<div id="test5" class="animate-obj">shake</div>
<button id="trigger5">点击触发动画 shake</button>

````js
seajs.use(['jquery', 'index.css'], function($) {
    $('#trigger5').click(function() {
        $('#test5').addClass('animated shake');
    });
});
````
