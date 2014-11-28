Images-Transfrom
=========

Some inspiration for article intro effects on headers and fullscreen images.

TransfromOne
=========
使用模糊效果有三种普遍的方法：

1、半透明模糊 PNG 覆盖的方式，这种方式简单易行，但是不能灵活控制模糊程度。

2、CSS方式，比如用-webkit-filter:blur(10px); 的形式，也极其简单，可控制模糊程度，但是这种方式的效果很差很差，中心模糊度高，四周模糊度低，而且整个元素外围会有光晕效果，已经不是真正意义的模糊了。

3、Javascript方式更新画布，最灵活，效果最好，自己写代码就复杂一点，但是已经有现成的js库可以使用了，简单调用函数即可。

推荐使用：[StackBlur V0.5](http://www.quasimondo.com/StackBlurForCanvas/StackBlurDemo.html)（不单是js，他的算法也可以运用到ios以及其他设备上）

这个库提供了三种参数：

	`stackBlurImage( sourceImageID, targetCanvasID, radius, blurAlphaChannel );    //用于将图片模糊绘制到canvas`

    stackBlurCanvasRGBA( targetCanvasID, top_x, top_y, width, height, radius );  //用于对Canvas矩形区域执行RGBA模糊

	stackBlurCanvasRGB( targetCanvasID, top_x, top_y, width, height, radius ); //用于对Canvas矩形区域执行RGB模糊，不考虑Alpha值


Demo
=========
图片模糊过渡效果[demo](http://myimages.oschina.mopaas.com)

图片变暗过渡效果[demo](http://myimages.oschina.mopaas.com/index2.html)

**[Jsfiddle Demo](http://jsfiddle.net/nwellcome/27QUM/)**
TransfromTwo
=========
使用简单的过渡效果加上Background实现类似Medium的效果

`background: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.5),rgba(0, 0, 0, 0.7));
`

[© Bibimap 2014]()