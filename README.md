# 11×11 困难关网站发布包

这是一个纯静态网页小游戏，打开 index.html 即可使用，不依赖外部字体、CDN、接口或数据库。

## GitHub Pages 发布

1. 在 GitHub 创建一个公开仓库，例如 cat-puzzle。
2. 上传本目录里的 index.html；有条件时也上传 .nojekyll。不要只上传 ZIP 压缩包。
3. 提交文件后，进入仓库 Settings → Pages。
4. Source 选择 Deploy from a branch；Branch 选择 main，目录选择 / (root)，保存。
5. 等待部署完成，Pages 页面会显示实际网站地址。把那个地址分享给其他人。

项目网站通常位于 https://用户名.github.io/仓库名/ 。如果仓库名是 cat-puzzle，就用对应的项目地址。

GitHub Pages 能发布此页面，但国内各地网络的访问速度和可达性需要实际测试，不能保证始终稳定。

## 需要面向国内用户稳定分享时

可选择国内云的静态网站托管或对象存储静态网站功能，上传 index.html 并将其设为默认首页。按服务商要求配置域名、HTTPS 和备案。源代码可以仍保存在 GitHub，网站托管位置可以独立选择。

## 文件说明

- index.html：完整可玩的游戏页面，包含题面、提示和答案核对功能。
- .nojekyll：告诉 GitHub Pages 直接发布静态文件。

原来的 http://127.0.0.1:8769/ 地址只指向打开链接的人自己的电脑，不能作为公网分享地址。

参考：
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
- https://cloud.tencent.com/document/api/436/9512
