# hugo-theme-pure 使用指南

[hexo-theme-pure](https://github.com/cofess/hexo-theme-pure) 移植版本. 简单,功能丰富使用.

## 参与

由于主要做后端开发,其实对前端(`CSS` 啥的)一窍不通,完全是硬着脑阔移植. 有些很喜欢的特性,并不知道怎么加,研究太久就会很浪费时间,所以如果你有很不错的 `feature` 希望能放上来,那是最好不过了.

`repo` 的文件结构大致是参考 [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure) 的,应该是比较清晰了. 可以根据你的需求针对性的修改.如果稍微看一下文件结构的话你会发现还有听过功能没有实现的.

## 特性

1. 多语言支持
2. 多种评论系统集成
3. 多种皮肤
4. 集成站内搜索(感谢[@ppoffice](https://github.com/ppoffice)提供的`insight.js`)

## 预览

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/grey.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/black.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/blue.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/green.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/purple.png)

## 安装

```bash
$ cd $HUGO_ROOT
$ git clone https://github.com/xiaoheiAh/hugo-theme-pure themes/pure
$ ./hugo server -t pure
```

### 注意

1. 请拷贝`exampleSite` 下的 `config.yml` 进行自定义配置.

2. 需要将你的博客文件放到 `content/posts` 文件夹下,才能渲染出来. 即: `./hugo new posts/blabla.md`

## 多语言支持

目前支持英语和中文两种语言,如需其他语言可以在 [i18n](i18n/) 目录下新增其他语言的 `yml` 文件,内容与现有的语言对应即可.

设置网页默认语言, `config.yml:`

```yml
defaultContentLanguage: zh # en,fr...
```

## 主题颜色及布局

修改下列配置

```yml
# config
config:
  skin: theme-black # 主题颜色 theme-black theme-blue theme-green theme-purple
  layout: main-center # 布局方式 main-left main-center main-right
```

## 图标

菜单栏有默认的图标展示,需要更换请参考 [Iconfont](http://blog.cofess.com/hexo-theme-pure/iconfont/demo_fontclass.html), 并更改相应的配置

```yml
menuIcons:
  enable: true  # 是否启用导航菜单图标
  home: icon-home-fill
  archives: icon-archives-fill
  categories: icon-folder
  tags: icon-tags
  repository: icon-project
  books: icon-book-fill
  links: icon-friendship
  about: icon-cup-fill
```

## 评论

目前支持三种评论: **Disqus**, **Gitalk**, **Valine**, 加上对应配置即可.

## 图片资源

图片资源放在static目录下即可,具体根据 `config` 配置.

```yml
site:
	favicon: favicon.ico
profile:
	avatar: avatar.png
```

## TOC

开启 toc

```yml
  # config
  config:
    toc: true
```

## 捐赠

支持支付宝,微信付款码,需要先将二维码截出来并存放在 `static` 目录下.目前默认是在 `static/donate`. 需要的配置如下:

```yml
# Donate
donate:
	enable: true
	# 微信打赏
	wechatpay:
		qrcode: donate/wechatpayimg.png
		title: 微信支付
	# 支付宝打赏
	alipay:
		qrcode: donate/alipayimg.png
		title: 支付宝
```

## License

Released under the [MIT](https://github.com/olOwOlo/hugo-theme-even/blob/master/LICENSE.md) License.

## 鸣谢

- [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure)

- [hugo-theme-even](https://github.com/olOwOlo/hugo-theme-even)

  

