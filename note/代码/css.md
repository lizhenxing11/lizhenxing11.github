# 字体
* font-size：字体大小
* font-family: 字体
* color：字体颜色
# 选择器
* .class 类别选择器
* #id    id选择器
* .class 子集   层级选择器
# 布局
* width：设置宽
* height：设置高
* text-align：center；元素横向居中
* line-height：高度；元素纵向居中
* float：浮动
* margin：上 右 下 左 外边框
* padding：内边框
* text-decoration:none; 下划线取消
* margin：0 auto；块元素横向居中(其中0可变XXpx改变上下外边框)
* overflow：hidden   隐藏多余元素（放在父集可以使子集加边框时不影响父集）
* overflow：auto；   隐藏并出现滚动条
* list-style：none；去掉li的点
* display：block；行内元素变成块元素
### 浮动
* float：left；左浮动
* float；right；右浮动
* .clear{clear: both;}  清除浮动   浮动元素后边加上<div class="clear"></div>
* .clear:befor,.clear:after{
	clear:both;
	content:;
}在名称里面加上clear可以清除前后浮动
# 名称
* header 头
* banner 图片轮播
* container 中间
* footer 结尾
# 边框
* border：--px solid 颜色；形成一定颜色的实现边框
* border：--px bashed 颜色；形成一点颜色的虚线边框
* border-radius：（）px 倒圆角
* box-sizing：border-box；把实宽变成width
#动画
* .box：hover{}鼠标悬浮变成什么样 需要父子级关系
* transform：；  转换
* transition：transform  5s   控制过渡效果(指定一个元素的某一个属性成过渡效果)
* rotate（deg）旋转
* scale（px）   缩放   正值是放大  负值是缩小
* translateX/Y()  平移
* @keyframes name{}   生成一个动画格式
* animation: 动画名字 2s；   执行一个动画
* linear   匀速
* infinite  无限循环
* prespective  视觉距离（加到那个div那个div变化）
* backface-visibility: hidden; 翻转到背面隐藏  需要配合prespective使用
* transform-style: preserve-3d;   让子集具有3d效果
# 表单
```
* <form action="提交的服务器" name="没有那么不能提交"></form>    表单
* <button></button>    <input type="button">按钮
* <input type="text">   文本框
* <input type="password">   密码
* <input type="radio" value="单选框里面的东西">   单选框
* <input type="checkbox">    多选框
* <input type="submit">     提交按钮
* <textarea name="" id="" cols="30行数" rows="10列数"></textarea>     文本域
* placeholder    文本框里添加字体  但当鼠标点到时文本消失
```
* 打断点 @media screen and（max-width（最大宽度））{要改变的样式}