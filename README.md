# Angel's Ladder 个性化配置

## Overview

Angel's Ladder is a simple blog theme for Hugo.
* Simple and clean design
* Responsive design
* Pagination
* Tagging
* Disqus
* Source code highlighting
* Google Analytics

个性化部分：
* 修改标题栏中 社交账户的配置参数，增加 微博，微信，简书，邮件，去除不常用的 Twitter、Facebook等国外社交账户
* 在页尾增加文字分类链接
* 增加首页文章简介（summary）
* 增加列表页文字简介（summary）



## Screenshot

![](https://github.com/chaomifan/anglesladder/blob/master/screenshot/1.png?raw=true)  


## Installation

将文件 Clone 到 hugo 的 themes 文件夹
```
cd themes
git clone https://github.com/chaomifan/anglesladder.git "angels-ladder"
```

使用皮肤文件夹中的 config.toml 文件 替换原本的 config 文件 (path/to/yoursite 是你 hugo 生成的网站存放路径)
````
mv web_config/config.toml path/to/yoursite/config.toml
````

预览效果（path/to/yoursite 是你 hugo 生成的网站存放路径）
````
cd path/to/yoursite
hugo server -t angels-ladder -D -w
````


## Configuration （config.toml）

**贴上我修改过的配置文件**

````
baseurl = "http://chaomifan.github.io/"
languageCode = "en-us"
title = "Ethan's PMbook"
theme = "angels-ladder"
disqusShortname = "Ethan's PMbook"

[params]
	subtitle = "信心是黑暗中的灯塔，任何时候都不能丢"
	about = "#"
	weibo = "http://www.baidu.com"
    wechat = "htttp://www.baidu.com"
	jianshu = "http://www.jianshu.com/users/f5820a96231b/timeline"
	github = "http://www.baidu.com"
	mail = "mailto:xielm@qq.com"
	guifan = "/categories/产品规范/"
	fenxi = "/categories/产品分析/"
	jiqiao = "/categories/技巧分析/"
	yanjiu = "/categories/技术研究/"
	profile = "/images/ethan.png"
	copyright = "Written by Ethan，转载请注明出处，谢谢！"
````


**原版皮肤中关于配置文件的修改说明**
To take full advantage of the features in this theme, you can add variables to your site config file.

The following is the example configuration.

````
baseurl = "http://tanksuzuki.com/"
languageCode = "ja"
title = "TANKSUZUKI.COM"
disqusShortname = "tanksuzuki"

[Params]
subtitle = "I would like to be a layer 3 switch."
facebook = "https://facebook.com/foobar"
twitter = "https://twitter.com/foobar"
github = "https://github.com/foobar"
showsRSS = true
profile = "/images/profile.png"
copyright = "Written by Asuka Suzuki"
analytics = "UA-XXXXXXXX-X"
shareThis = "XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX"
````

Details of each parameter are as follows.

| Parameter | Required | Comment |
| :--- | :--- | :--- |
| baseurl | yes | Enter the title of your site. |
| languageCode | yes | Enter the language code of HTML. Example: en, ja. |
| title | yes | Enter the title of your site. |
| disqusShortname | no | Enter the short name of the disqus. If you do not enter, disqus section is hidden. |
| subtitle | no | Enter the subtitle of your site. If you do not enter, subtitle is hidden. |
| facebook | no | Enter the URL of Facebook. If you do not enter, the link is hidden. |
| twitter | no | Enter the URL of Twitter. If you do not enter, the link is hidden. |
| github | no | Enter the URL of Github. If you do not enter, the link is hidden. |
| showsRSS | no | Enter true to show the URL of RSS. If you enter false or nothing, the link is hidden. |
| profile | no | Enter the path to the profile image. If you do not enter, profile section will be hidden. |
| copyright | no | Enter the copyright notice. If you do not enter, copyright display is hidden. |
| analytics | no | Enter the tracking ID of Google analytics. If you do not enter, the analysis will be skipped. |
| shareThis | no | Enter the publisher key of ShareThis. If you do not enter, the ShareThis buttons are hidden. 


## Style Customization

To change the theme color, edit the `layouts/static/theme.less`.
Then compile the LESS file by using [one of LESS compilers](http://leafo.net/lessphp/editor.html),
and replace the content of `layouts/static/theme.css` with the compiled CSS.

The default theme color is `#29abe2`.
Please change the favorite color.

````
/* Theme color
--------------------------------------------------*/
@color: #29abe2;
````

For original styles, please edit the `layouts/static/custom.css`.


## License

Open sourced under the [MIT license](https://github.com/tanksuzuki/angels-ladder/blob/master/LICENSE.md).


## Author

* 原作者：Asuka Suzuki
* 修改：Ethan 

## 参考文档
> gohugo.io/content/summaries/
> www.gohugo.org/theme/angles-ladder/

## Contact

[点此给我发邮件](mailto:xielm@qq.com)   :）


