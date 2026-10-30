# Yinming Wang's Homepage

我的个人主页源码。在线访问：<https://yinming-wang.github.io/>

基于 [Yixin Huang 的个人主页模板](https://github.com/Yixin0313/personal-homepage-template)（MIT License）修改。

## 目录结构

```text
.
├── index.html              # 页面骨架，一般只需要改导航和页脚链接
├── contents                # 页面文字内容（改这里就够了）
│   ├── config.yml          # 网站标题、副标题、版权信息
│   ├── home.md             # 首页：个人简介、邮箱、教育经历、研究方向
│   ├── awards.md           # 获奖经历
│   ├── experience.md       # 工作 / 项目经历
│   └── publications.md     # 论文发表
└── static
    └── assets/img          # photo.jpg（头像）、background.jpg（页面顶部背景）
```

## 修改内容

1. 编辑 `contents/config.yml`：网站标题、导航栏名称、顶部标语、版权信息。
2. 编辑 `contents/*.md`：各板块正文。页面会把这些 Markdown 文件渲染到对应板块中。
3. 替换 `static/assets/img/photo.jpg`（头像）和 `background.jpg`（顶部背景，页面会自动裁成 1920×400 的横幅）。
4. 如需增删板块，同时修改 `index.html` 中的 `<section>`、导航栏和 `static/js/scripts.js` 里的 `section_names`。

## 本地预览

页面通过 JavaScript `fetch` 读取 `contents/*.md`，直接双击 `index.html`（`file://`）会被浏览器的跨域策略拦截，需要启动一个本地服务器：

```bash
cd Yinming-Wang.github.io
python -m http.server 8000
```

然后打开 <http://localhost:8000>。改完内容后刷新浏览器即可看到效果，按 `Ctrl+C` 停止服务器。

## 发布

```bash
git add .
git commit -m "Update homepage content"
git push
```

推送到 `main` 分支后，GitHub Pages 会在 1–2 分钟内自动重新部署，访问 <https://yinming-wang.github.io/> 即可看到最新版本。

## License

MIT License，版权声明见 [LICENSE](LICENSE)。
