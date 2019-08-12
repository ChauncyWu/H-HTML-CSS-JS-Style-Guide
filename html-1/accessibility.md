# Accessibility

###  国际残疾人日

12月3日的“国际残疾人日”\(International Day of Disabled Persons\)是一年一度的活动，旨在促进人们对残疾问题的理解和动员人们支持维护残疾人的尊严、权利和幸福。1992年10月12日至13日，第47届联合国大会举行了自联合国成立以来首次关于残疾人问题的特别会议。大会通过决议，将每年的12月3日定为“国际残疾人日”。（引自百度百科）

### WAI-ARIA

Web Accessibility Initiative - Accessible Rich Internet Applications：可访问的富互联网应用

## a 标签相关

### a 标签的`href`属性

问：button标签由于其在各个平台初始样式的多样性难以编写一致样式，往往使用a标签去模拟一个按钮。为什么不用div或者其他标签模拟呢？

答：button标签支持键盘导航（即使用Tab键定位），a标签在设置href属性后也支持该特性，而且天然鼠标手型，而其他标签需要做额外操作，故使用a标签进行模拟。

问：a标签的`href`属性值该设置成什么？

答：约定该写法 `href=“javascript:;”`，具体区别参考以下链接。

* [&lt;a href="javascript:void\(0\)"&gt;这样写为什么不好?](https://segmentfault.com/q/1010000000339082)
* [疑问：为什么要使用href=”javascript:void\(0\);”?](https://www.zhangxinxu.com/wordpress/2013/01/why-use-href-javascript-void0/)

### a 标签的 role 属性

考虑设置role="button"，这样在屏幕阅读器下就会读出“XX按钮”而不会读成“XX链接”

### a 标签模拟按钮下的 hover 和 focus 状态

平常在编写按钮样式时经常会写hover的状态，而hover是鼠标经过的样式，考虑到在无鼠标情况只能使用Tab键，而Tab键定位到该按钮时是focus状态，故考虑在编写focus样式与hover样式一致。

## 关于页面在 img 、CSS 和 JS 加载失败情况下的可访问性

1. 使用chrome插件disable-HTML可以查看在未加载img、css或js等情况下页面的显示情况。
2. 尽管一些按钮或者标题经常使用图片来替代，但是按钮和标题上对应的文字还是需要写上，以免在图片没有加载出来的情况下一片空白，可以使用`text-indent: -999em; overflow: hidden;`来隐藏文字，对于一些没必要显示的文字可以设置`font-size: 0;`

## 排版相关

1. 行高至少为字体大小的1.5倍；
2. 段落下方的空间至少为字体大小的2倍；
3. 字母间距至少为字体大小的0.12倍；
4. 字间距至少为字体大小的0.16倍；

## 控件相关

1. 确保交互式元素的大小至少为44px\*44px；
2. 如果有功能需要用户摇动、倾斜或手势操作，则需提供有相同功能的表单控件；
3. 使用label标签的for+id方式扩展表单控件的可点击区域；

## 参考文档

* [Web Content Accessibility Guidelines \(WCAG\) 2.1](https://www.w3.org/TR/WCAG21/)
* [Web Content Accessibility Guidelines 2.1—for People Who Haven’t Read the Update](https://24ways.org/2018/wcag-for-people-who-havent-read-the-update/)
* [Web 可访问性整理](https://blog.crimx.com/2017/12/08/web-accessibility/)
* [可访问性文章\|张鑫旭](https://www.zhangxinxu.com/wordpress/tag/%E5%8F%AF%E8%AE%BF%E9%97%AE%E6%80%A7/)
* [ARIA属性表](https://www.zhangxinxu.com/wordpress/2012/03/wai-aria-%E6%97%A0%E9%9A%9C%E7%A2%8D%E9%98%85%E8%AF%BB/)

