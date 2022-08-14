### docsify配置

```html
<body>
  <div id="app"></div>
  <script>
    window.$docsify = {
      name: '',|网站标题
      logo: '',|网站图标地址,可用CSS更改大小：
        '<img src="XXX.png/jpg" alt="logo" style="zoom:45%;" />'
      repo: 'username/repo',|页面右上角GitHub挂件
      nameLink: '',|点击文档标题跳转的链接地址
      loadNavbar: true/false,|导航栏，默认' _navbar.md',可自定义
      loadSidebar: true/false,|侧边栏，默认'_sidebar.md'，可自定义
      hideSidebar: true/false,|隐藏侧边栏
      subMaxLevel: '',|侧边栏目录最大层级
      auto2top: true/false,|切换页面后是否跳转到页面顶部
      homepage: '',|首页，默认'EADME.md'，可自定义
      relativePath: true/false,|相对路径，在该同路径下寻找文件
      coverpage: true/false,|封面页,默认'_coverpage.md'
      autoHeader: true/false,|侧边栏自动添加标题
      noEmoji: true/false,|禁用 emoji 解析
      externalLinkTarget: '_self',|外部链接打开方式，默认'_blank'(新窗口)
      cornerExternalLinkTarget: '_self',|右上角链接打开方式，默认'_blank'(新窗口)
      externalLinkRel: '',|默认'noopener'可以防止新打开的外部页面（当'externalLinkTarget'为'_blank'时）能够控制我们的页面，没有设为'_blank'的话就不需要设置了
      mergeNavbar: true/false,|小屏设备合并导航栏到侧边栏
      onlyCover: true/false,|只在访问主页时加载封面
      ext: '.md',|资源的文件扩展名
      notFoundPage: true/false,|404，默认'_404.md',可自定义
      topMargin: 0,|指定目录，文章标题移动至距页顶的多余空间
      count:{
        countable:true,
        fontsize:'0.9em',|字体大小
        color:'rgb(90,90,90)',
        language:'chinese'|语言
      }|配合<script src="//unpkg.com/docsify-count/dist/countable.js"></script>
    }
  </script>
```

```html
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/emoji.min.js"></script>
```

如果不想解析成表情符号，可使用'__colon__'或'&#58；如果需要在标题中使用，建议使用&#58。例，`&#58;100:'

```html
<script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/zoom-image.min.js"></script>
```

图片缩放

```markdown
![](XXX.png ":no-zoom")
忽略某张图片
```

```html
<script src="//cdn.jsdelivr.net/npm/docsify-copy-code/dist/docsify-copy-code.min.js"></script>
```

在代码块上添加Click to copy按钮来轻易地复制代码

```html
<script src="//cdn.jsdelivr.net/npm/prismjs@1/components/prism-bash.min.js"></script> 
<script src="//cdn.jsdelivr.net/npm/prismjs@1/components/prism-php.min.js"></script>
```

代码高亮|需要在代码块第一行添加对应的语言声明

````markdown
```html
```
````

