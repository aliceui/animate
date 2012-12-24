# 演示文档

---

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
seajs.use(['$', '../src/animate.css'], function($) {
    $('#trigger1').click(function() {
        $('#test1').addClass('animated bounceOutLeft');
    });
});
````

<div id="test2" class="animate-obj"></div>
<button id="trigger2">点击触发动画</button>

````js
seajs.use(['$', '../src/animate.css'], function($) {
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
seajs.use(['$', '../src/animate.css'], function($) {
    $('#trigger3').click(function() {
        $('#test3').addClass('animated rotateInUpRight');
    });
});
````
