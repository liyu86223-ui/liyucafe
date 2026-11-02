# 生活本 · 一杯一日

饮品、吃饭和购物的日常记录。纯静态网页，无需安装依赖或构建。

## 上传到 GitHub 并开启 Pages

1. 新建 GitHub 仓库。
2. 将本文件夹**里面的文件和 icons 文件夹**上传到仓库根目录。打开仓库时应直接看到 `index.html`；不要把外层 `github-pages` 文件夹整体套进去，也不要只上传 ZIP。
3. 打开仓库 **Settings → Pages**。
4. 在 **Build and deployment → Source** 选择 **Deploy from a branch**。
5. Branch 选择上传文件所在分支（通常为 **main**），目录选择 **/(root)**，点击 **Save**。
6. 发布完成后，在同一页打开显示的网站网址，用手机访问该 HTTPS 网址。

官方说明：[GitHub Pages 发布来源设置](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)

## 手机上试用

- 用手机浏览器打开发布后的网址，可通过浏览器菜单添加到主屏幕；已附主屏幕图标与独立窗口配置。
- 浏览器与“添加到主屏幕”后的储存空间可能不同，建议选定一种入口持续记录。
- 饮品价格可留空，吃饭、购物需填写金额；三类记录都可拍照/选照片并制作贴纸。
- 照片抠图在浏览器中处理，首次需联网下载第三方模型，速度取决于网络与手机性能。失败时保留原照片，可重试或使用原图。
- 此发布包未配置离线缓存，打开网页与首次加载抠图资源需要网络。

## 记录与备份

- 记录和照片保存在当前设备、当前浏览器的网站储存中，无账号、无自动云同步。
- 上传此发布包不会带入电脑预览中的记录，也不会把手机记录提交到 GitHub。
- 迁移电脑上的记录：在原预览页的设置中导出备份，再在手机发布页的设置中导入。
- 换设备、换浏览器、换网址或清除浏览器网站数据前，请先在设置中导出备份。日常也建议定期备份。
- 后续更新时覆盖发布文件即可；保持原网址与浏览器通常会保留已有记录，更新前仍建议导出备份。

## 文件

- `index.html`：完整应用。
- `manifest.webmanifest`：主屏幕名称、图标与启动路径。
- `icons/`：SVG 网站图标、PNG 主屏幕图标。
- `.nojekyll`：让 GitHub Pages 直接发布静态文件。

所有本地资源使用相对路径，可部署在 GitHub Pages 的仓库子路径下。

## 第三方组件

自动抠图按需加载 [IMG.LY background-removal-js](https://github.com/imgly/background-removal-js) 1.7.0（AGPL-3.0），以及其模型和运行时。应用设置中保留了组件来源链接。
