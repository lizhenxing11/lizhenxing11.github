# 移动端代码
```html
<meta name="viewport"（视图） content="width=device-width（手机屏幕分辨率）, user-scalable=no, （不能缩放）initial-scale=1.0,（原始比例	） maximum-scale=1.0, minimum-scale=1.0">
这是移动端必须的东西  
```
```javascript
使页面的单位按屏幕尺寸可调节
(function (doc, win) {
var docEl = doc.documentElement,
  resizeEvt = 'orientationchange' in window ? 'orientationchange' : 'resize',
  recalc = function () {
    var clientWidth = docEl.clientWidth;
    if (!clientWidth) return;
    docEl.style.fontSize = 100 * (clientWidth / 720设计稿的尺寸) + 'px';
  };
if (!doc.addEventListener) return;
win.addEventListener(resizeEvt, recalc, false);
doc.addEventListener('DOMContentLoaded', recalc, false);
})(document, window);
```
* initial-scale：初始缩放比例，也即是当页面第一次 load 的时候缩放比例。
* maximum-scale：允许用户缩放到的最大比例。
* minimum-scale：允许用户缩放到的最小比例。
* user-scalable：用户是否可以手动缩放
* ```
<script src="引用的js文件名"></script>
#### 单位
* px 固定单位
* em   随着父级的改变变大    等于父级font-size×乘本身的值（px）
*  rem   随着html的改变变大    等于htmlfont-size×乘本身的值（px）
