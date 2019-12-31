# hugo-theme-pure

A port of [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure) for Hugo. Powerful & Clean. [Iconfont](http://blog.cofess.com/hexo-theme-pure/iconfont/demo_fontclass.html)

[简体中文](README-ZH.md)

## Contribute

Since I mainly do back-end development, I don’t know anything about the front-end (`CSS` or something). It’s a hard-hitting transplant. Some of the features that I like very much don’t know how to add it. It’s a waste of time to study too long, so If you have a very good `feature` and hope to put it up, it would be best.

The file structure of `repo` is roughly referred to [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure) and should be clearer. It can be modified according to your needs. If you look at the file structure a little, you will find that the function has not been implemented.

## Changelog

1. [2019-11-19] Add `mainSections` param to avoid hard code.You can set this param to choose which directory under your content folder you want to render. `posts` by default. You can also unset it,but there seems have some problem.

2. [2019-11-19] Support MathJax([PR](https://github.com/xiaoheiAh/hugo-theme-pure/pull/20)) Reference:[MathJax-With-Hugo](https://gohugo.io/content-management/formats/#mathjax-with-hugo)& Upgrade jQuery version([PR](https://github.com/xiaoheiAh/hugo-theme-pure/pull/19)).

   e.g. 

   ```latex
   $$\begin{cases}
   a_1x+b_1y+c_1z=d_1\\
   a_2x+b_2y+c_2z=d_2\\
   a_3x+b_3y+c_3z=d_3\\
   \end{cases}
   $$
   ```

     <img src="https://raw.githubusercontent.com/xiaoheiAh/imgs/master/20191121103534.png" alt="not-set-mmark" style="zoom:50%;" />
   <img src="https://raw.githubusercontent.com/xiaoheiAh/imgs/master/20191121104118.png" alt="set-mmark" style="zoom:50%;" />

3. [2019-12-07] beautify toc by [tocbot](https://github.com/tscanlin/tocbot/)

4. [2019-12-24] support pagination

5. [2019-12-31] 
   1. support highlight shortcode Note: Just compatible with basic `highlight` usage like:
   
      ```html
      {{< highlight go >}}
      // ... code
      {{< / highlight >}}
      ```

     If you use hugo official example like,rendering will be very ugly.I don't want to compatible with it or maybe you want. Don't forget send a pr~ thanks.
   
     ```html
      {{< highlight go "linenos=table,hl_lines=8 15-17,linenostart=199" >}}
      // ... code
      {{< / highlight >}}
     ```
   
   2. Minify css&js file.

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

## TOC

enable toc 

```yml
  # config
  config:
    toc: true
```



## TODO

- [x] TOC
- [x] pagination

## License

Released under the [MIT](https://github.com/olOwOlo/hugo-theme-even/blob/master/LICENSE.md) License.

## Acknowledgements

- [hexo-theme-pure](https://github.com/cofess/hexo-theme-pure)

- [hugo-theme-even](https://github.com/olOwOlo/hugo-theme-even)

  

