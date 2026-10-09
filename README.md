# Zizhuo Lin · 林子卓

简洁的个人学术主页，地址：https://zerovector1201.github.io/ZizhuoLin.github.io/ 。

纯 HTML + CSS，无构建依赖、远程字体、追踪脚本或 JavaScript。论文的“Method & results”使用浏览器原生折叠面板，支持键盘操作。页面适配桌面与手机。

## 修改内容

- `index.html`：个人简介、联系方式、研究、教育背景与荣誉。
- `assets/style.css`：字体、颜色、间距与移动端布局。
- `assets/favicon.svg`：浏览器图标。
- `assets/figures/`：五篇论文的主图与预览缩略图（CCOPD 使用第 5 页 Figure 3，ParticleGS 使用第 3 页 Figure 2，其余使用 Figure 1）；图源与裁切信息见 `assets/figures/SOURCES.md`。
- `sitemap.xml`：更新页面时同步修改 `lastmod`。

内容依据工作区的本人简历整理。论文作者角色与状态沿用该简历；页面中的姓名行用于说明本人贡献角色，不是完整作者名单。论文公开后，可在对应 `article` 中补充完整作者与 Paper / Code 链接。

当前版本使用英文正文与中文姓名；ToM-Video 显示 EMNLP 2026 Main 已录用，Trajectory Dropout 和 CCOPD 统一显示 Under review。未填入未提供的导师或个人照片。

2026-10-09 根据本人 [Google Scholar](https://scholar.google.com/citations?hl=zh-CN&user=D-OS9K4AAAAJ) 列表补入两篇合作论文：Part-X-MLLM（ICLR 2026）与 ParticleGS（CVPR 2026 Highlight）。作者顺序、年份和标题与官方论文交叉核对，Highlight 标记依据作者官方代码仓库。完整来源见 `PUBLICATION-SOURCES.md`。个人信息区同步加入 Google Scholar 链接。

论文区优先按桌面端设计：左侧约 286px 的主图，右侧标题、状态、作者角色和简介。点击主图可在新标签页打开高清 PNG；小屏改为上下排版。预览图按原比例完整展示，页面只加载较小的缩略图，点击时才加载高清图。

## 本地预览

直接打开 `index.html` 即可，也可以在此目录运行：

```powershell
python -m http.server 4173 --bind 127.0.0.1
```

浏览器访问 `http://127.0.0.1:4173`。

## GitHub Pages 托管

这个目录是 `ZeroVector1201/ZizhuoLin.github.io` 仓库的独立克隆。

1. 将更改提交并推送至该仓库的 `main` 分支。
2. 在仓库 **Settings → Pages → Build and deployment**，选择 **Deploy from a branch**。
3. 选择 **main** 与 **/ (root)** 并保存。若已有该配置，无需重复设置。
4. 等待 GitHub Pages 部署完成，访问 `https://zerovector1201.github.io/ZizhuoLin.github.io/`。

站点入口保留在仓库根目录，适配现有主页的分支发布方式；`.nojekyll` 让文件以静态资源发布，无需另建工作流。请仅推送此目录，不要将上层简历工作区纳入网站仓库。

参考：[GitHub 官方 Pages 发布源说明](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)。
