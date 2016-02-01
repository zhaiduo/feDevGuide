# feDevGuide
本项目搜集整理了目前最常用的前端开发规范，希望对自定自己的前端开发规范有所帮助。

##HTML开发规范
```
> 要求兼容W3C HTML5规范（验证地址：https://validator.w3.org/）
> 必须包含HTML5 Polyfills补丁，用以支持低版本浏览器
    https://github.com/afarkas/html5shiv
    https://github.com/Modernizr/Modernizr/wiki/HTML5-Cross-Browser-Polyfills
> Doctype统一为 <!doctype html>
> head title之前必须包含utf8编码 <meta charset="UTF-8">
> 缩进控制为2-4个空格
> HTML头部只能放置CSS文件和必需的js初始化内容，其它js脚本全部放在网页底部，按src引用，尽量不要在页面中写脚本。
> 浏览器样式兼容推荐使用如下方式：
    var doc = document.documentElement;
    var ua = navigator.userAgent.replace(/[^0-9a-z,; _\(\)\/\.\-]/ig,"");
    doc.setAttribute('data-useragent', ua);

    通过规则匹配对应浏览器样式：html[data-useragent*='iPhone'] .target{}
> html标签内不得使用js事件，如onclick等，所有事件尽量在js脚本中完成（angular这种双向绑定框架除外）
```

##CSS样式表开发规范
```
Google HTML/CSS Style Guide
https://google.github.io/styleguide/htmlcssguide.xml

CSS coding styleguide
https://pages.18f.gov/frontend/css-coding-styleguide/

Airbnb CSS / Sass Styleguide
https://github.com/airbnb/css

> 为了语义化，方便识别样式定义的功能，样式名称按小写字母（可缩写：pt = padding-top）加-来分隔的方式
> 为了和第三方项目样式区分，本公司自定义样式推荐以pb-开头（除了已使用的样式规则）
> 目前使用的样式规则
    c开头的样式表示: caaaaaa => #aaaaaa
    f开头的样式表示: f14 => font-size:14px
    pt开头的样式表示: pt20 => padding-top:20px
    mt开头的样式表示: mt20 => margin-top:20px
> 常用通用样式
    noselect: 禁止选中文本的样式
> CSS文件结构顺序：
    0.通用样式
    1.普通样式
    2.响应式样式
    3.针对浏览器的样式
> 样式按theme主题区分
> 结构布局和颜色、大小分离
> 绝对定位和相对定位分离
> 其它规则以组件化、可重用化为准
> 两条样式分行放，不用放在同一行
> 样式尽量模块化，以便不同页面引用
> 样式能简写就简写
```

##LESS样式表开发规范

##SASS样式表开发规范

##Javascript开发规范
```
Airbnb JavaScript Style Guide
https://github.com/airbnb/javascript#table-of-contents
https://github.com/airbnb/javascript/tree/master/es5

Google JavaScript Style Guide
https://google.github.io/styleguide/javascriptguide.xml

> 所有js脚本建议用sublime开发，使用插件（javascript beautify）格式化js脚本(ctrl+alt+F)
```

##Jquery开发规范

##Angular开发规范

##ES5开发规范

##NodeJs开发规范
https://github.com/felixge/node-style-guide

###相关参考
```
> http://www.jslint.com/help.html
```

###
本文档将不断更新，欢迎大家查漏补缺。




