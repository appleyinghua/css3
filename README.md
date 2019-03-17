# css3
CSS3新的特性学习
包括文本阴影、圆角边框、渐变特性及多背景图片。动态特性包括过度、动画和变形。
text-shadow:水平偏移 垂直偏移 阴影距离 颜色；
text-shadow: 10px 10px 10px rgba(0,0,0,0.7);
设置多个阴影，模糊距离不同，产生辉光的效果
text-shadow: 0 0 1px #fff, 0 0 5px #fff, 0 0 10px yellow;
设置多个阴影，偏移方向不同，产生浮雕的效果
 text-shadow: -1px -1px 0 #fff, 1px 1px 0 #333, 2px 2px 0 #444;
多背景设置：background：url('')  left top no-repeat，url('') center center repeat;
线性渐变：绘制渐变时，会被浏览器解析成一张背景图片，所以属性为background-image: -webkit-linear-gradient(left,lightgray,lightgreen 50%, yellow);
径向渐变： background-image: -webkit-radial-gradient(center center,orange, yellow 40%,white);
圆角边框：border-radius 设置大小为宽度的一半就是半圆了。
动态特性：过度、动画、移动、旋转
过度：transition： all  执行时间    速率   延迟时间；【鼠标移入，移出等】
-webkit-transition:all 1s linear 1s;
动画：@-webkit-keyframes 过度名{  }
@-webkit-keyframes active {
            from { left: 0px;top:140px; }
            to { left: 600px;top:140px; }
        }
 -webkit-animation: active 5s infinite linear;
-webkit-animation: 过度名  执行时间  是否循环  速率;
移动：transform：translate（x,y）;
旋转：transform：rotate(30deg);
