# Personal Homepage

一个可以直接通过 GitHub Pages 发布的静态个人主页。白底、红色分节标题、顶部头像与简介、经历和论文区域均已搭好；所有个人信息均为 `[占位符]`。

## 文件

- `index.html`：页面内容，按章节编辑即可。
- `style.css`：字体、颜色、间距和手机端布局。
- `.nojekyll`：直接发布静态文件，无需 Jekyll 或构建工具。

## 逐步填写内容

1. 在 `index.html` 中替换方括号内的文字，包括页面标题、描述、姓名和页脚。
2. 头像准备好后，将 `.portrait` 占位容器替换为 `<img class="portrait" src="[照片文件路径]" alt="[照片说明]">`，并将图片放入仓库。
3. 联系方式、机构和论文链接目前是普通文本，不会跳转。准备好后，将对应的 `<span class="link-placeholder">[链接名称]</span>` 替换为 `<a href="[真实链接]">[链接名称]</a>`；邮箱链接的 `href` 使用 `mailto:` 加实际邮箱地址。
4. 教育、工作、研究经历可以复制对应的 `<article class="entry">` 添加；论文可以复制 `<article class="publication">` 添加。不需要的条目或章节可以整块删除。
5. 论文图片准备好后，将 `.publication-image` 占位容器替换为 `<img class="publication-image" src="[图片文件路径]" alt="[图片说明]">`。

## 预览和发布

可以直接在浏览器打开 `index.html`，也可以在仓库目录运行 `python3 -m http.server 8000` 后通过本地浏览器预览。

GitHub Pages 使用仓库的 **main** 分支、**/ (root)** 目录发布。修改后提交并推送到 `main`，等待 Pages 部署完成即可。

页面不依赖 JavaScript、第三方字体、外部图片或访客统计服务。
