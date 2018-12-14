# Code Standards

### 1. HTML5 doctype

```markup
<!DOCTYPE html>
```

### 2. 不要在自动闭合标签结尾处使用“/”

```markup
# Not recommended
<br/>

# Recommended 
<br>
```

### 3. 多媒体回退

```markup
# Not recommended
<img src="cw.png">

# Recommended 
<img src="cw.png" alt="describe of the picture">
```

### 4. 引入CSS，JS时省略type属性

```markup
# Not recommended
<link rel="stylesheet" href="main.css" type="text/css">
<script src="main.js" type="text/javascript"></script>

# Recommended 
<link rel="stylesheet" href="main.css">
<script src="main.js"></script>
```

### 5. 属性上使用双引号，而不是单引号

```markup
# Not recommended
<a class='main-button'>Sign in</a>

# Recommended 
<a class="main-button">Sign in</a>
```

### 6. 属性名全小写，用中划线做分隔符

### 7. lang属性

[HTML5规范推荐：](http://w3c.github.io/html/semantics.html#the-html-element)

> 应在html标签上加上lang属性。这会给语音工具和翻译工具帮助，告诉它们应当怎么去发音和翻译。

```markup
参考Aoto.io规范
# Recommended 
# 推荐使用属性值 cmn-Hans-CN（简体, 中国大陆）
# 但是考虑浏览器和操作系统的兼容性，目前仍然使用 zh-CN 属性值
<html lang="zh-CN">
// zh-CN与zh-cn相同

# 其他地区
zh-SG 中文 (简体, 新加坡)   对应 cmn-Hans-SG 普通话 (简体, 新加坡)
zh-HK 中文 (繁体, 香港)     对应 cmn-Hant-HK 普通话 (繁体, 香港)
zh-MO 中文 (繁体, 澳门)     对应 cmn-Hant-MO 普通话 (繁体, 澳门)
zh-TW 中文 (繁体, 台湾)     对应 cmn-Hant-TW 普通话 (繁体, 台湾)

# 20181211其他网站参考
- 维基百科
<html lang="zh-Hans-CN">

- facebook
<html lang="zh-Hans">

- twitter
<html lang="zh-cn">

- Google
<html lang="zh">
```

* 更多参考[网页头部的声明应该是用 lang="zh" 还是 lang="zh-cn"？](https://www.zhihu.com/question/20797118?utm_source=weibo&utm_medium=weibo_share&utm_content=share_question&utm_campaign=share_sidebar)

### 8. 字符编码

通过声明一个明确的字符编码，让浏览器轻松、快速的确定适合网页内容的渲染方式，通常指定为'UTF-8'

```markup
# Recommended 
<!DOCTYPE html>
<html>
 <head>
     <meta charset="UTF-8">
 </head>
 ...
</html>
```

### 9. 配置相关的meta标签

[常用meta整理](https://www.chauncywu.com/?p=148)

### 10. 属性顺序

属性应该按照特定的顺序出现以保证易读性；

* `class`
* `id`
* `name`
* `data-*`
* `src`, `for`, `type`, `href`, `value` , `max-length`, `max`, `min`, `pattern`
* `placeholder`, `title`, `alt`
* `aria-*`, `role`
* `required`, `readonly`, `disabled`

class是为高可复用组件设计的，所以应处在第一位；

id更加具体且应该尽量少使用，所以将它放在第二位。

### 11. boolean属性

 boolean属性指不需要声明取值的属性，XHTML需要每个属性声明取值，但是HTML5并不需要；

{% hint style="info" %}
 boolean属性的存在表示取值为true，不存在则表示取值为false。
{% endhint %}

```markup
<input type="text" disabled>

<input type="checkbox" value="1" checked>

<select>
    <option value="1" selected>1</option>
</select>
```

### 12. 

