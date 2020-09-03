自定义View的分类

继承View，继承ViewGroup、继承特定的View，比如TextView、继承特定的布局，比如LinearLayout。

如何自定义一个View？

1、明确需要继承的View是什么？如果是继承View类，需要处理padding不生效的问题，还有warp_content的问题，wrap_content默认与match_parent相同的；

2、添加View的构造方法，

3、重写父类的方法，比如onDraw，

4、如果有必要，自定义View的三个核心方法，