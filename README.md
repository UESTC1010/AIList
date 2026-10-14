# AI 探新社

好用的 AI，比你知道的更多。

网站正式地址：**[https://tanxinshe.cn/](https://tanxinshe.cn/)**

AI 工具导航与精选介绍，包含 6 个分类、44 个工具介绍页和 4 篇文章。支持搜索、分类筛选、浏览器收藏和手机访问。

## 网站文件

- `ai-tanxinshe-site.zip` 保存完整网站，包括 HTML、样式、脚本、封面和可编辑的内容 JSON。
- `.github/workflows/pages.yml` 在 `main` 分支更新时自动解压、检查并发布到 GitHub Pages。

## 更新内容

1. 下载并解压 `ai-tanxinshe-site.zip`。
2. 在 `ai-tanxinshe/content/tools.json` 或 `articles.json` 修改内容。
3. 在 `ai-tanxinshe` 目录运行 `node build.mjs` 和 `node check.mjs`。
4. 把整个 `ai-tanxinshe` 文件夹重新压缩成 `ai-tanxinshe-site.zip`，压缩包内需保留这个顶层文件夹。
5. 用新压缩包替换仓库中的同名文件，提交后自动发布。

无需安装 npm 包或配置 API 密钥。收藏保存在访问者自己的浏览器，不上传到本站。工具介绍基于官方资料，站内提供来源链接。

## 自定义域名

在仓库 **Settings → Pages → Custom domain** 中设置 `tanxinshe.cn`，在西部数码将根域名解析到 GitHub Pages，并将 `www` 的 CNAME 指向 `uestc1010.github.io`。DNS 检查通过且证书可用后，启用 **Enforce HTTPS**。

网站源文件 `ai-tanxinshe/content/site.json` 的 `baseUrl` 为 `https://tanxinshe.cn/`，页面 canonical 链接、站点地图和 robots.txt 使用此正式地址。当前通过 GitHub Actions 部署，无需在压缩包或仓库中添加 `CNAME` 文件。具体 DNS 记录见 [GitHub 官方自定义域名说明](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)。
