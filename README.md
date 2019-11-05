# hugo-theme-pure

A port of [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure) for Hugo. Powerful & Clean. [Iconfont](http://blog.cofess.com/hexo-theme-pure/iconfont/demo_fontclass.html)

[简体中文](README-ZH.md)

## Screenshots

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/grey.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/black.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/blue.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/green.png)

![](https://raw.githubusercontent.com/xiaoheiAh/hugo-theme-pure/master/images/purple.png)

## Installation

```bash
$ cd $HUGO_ROOT
$ git clone https://github.com/xiaoheiAh/hugo-theme-pure themes/pure
$ ./hugo server -t pure
```

### **Note** 

1. Please copy the config.yml under the `exampleSite` folder to the root folder of your Hugo Site. Feel free to change it. If you don't like `.yml` file, you can also convert it to you want.

2. Your post should under the `posts` folder, like this : `hugo new posts/any.md`

## Multilingual

Translations are collected from the [`themes/even/i18n/`](https://github.com/olOwOlo/hugo-theme-even/tree/master/i18n) folder (built into the theme), as well as present in `i18n` at your root of project.

You can specify `defaultContentLanguage` to use translations.

```yml
defaultContentLanguage: zh # en,fr...
```

Currently supports English and Chinese, you can see `en.yml` and `zh.yml` under `pure/i18n`. If you want to support other language, you can copy any yml file under `i18n` and rename to new language, then feel free to translate.

## Favicon & Images

You should put you images into `static` folder at your root project. When specify `favicon` or `donate qr code` , don't use absolute url like `/favicon.ico`, please use relative url like `favicon.ico` or `donate/alipay.png`

## Menu Icons

You can configure the menu according to the icons of [Iconfont](http://blog.cofess.com/hexo-theme-pure/iconfont/demo_fontclass.html), the following is configuration.

```yml
menuIcons:
  enable: true  
  home: icon-home-fill
  archives: icon-archives-fill
  categories: icon-folder
  tags: icon-tags
  repository: icon-project
  books: icon-book-fill
  links: icon-friendship
  about: icon-cup-fill
```



## TODO

- [ ] TOC
- [ ] pagination

## License

Released under the [MIT](https://github.com/olOwOlo/hugo-theme-even/blob/master/LICENSE.md) License.

## Acknowledgements

- [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure)

- [hugo-theme-even](https://github.com/olOwOlo/hugo-theme-even)

  

