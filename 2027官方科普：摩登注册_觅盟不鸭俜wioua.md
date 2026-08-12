摩登注册【Q-——333307——】摩登注册【 辋芷《888yx●vip》 】
摩登注册【Q-——333307——】摩登注册【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

关键词：GitHub Pages搭建博客 | Hexo教程 | 免费个人网站 | 静态博客部署 | 前端开发

你是否想拥有一个属于自己的技术博客，却苦于服务器费用和复杂配置？GitHub Pages 免费托管 + Hexo 极速生成静态页面，是开发者最优雅的解决方案。本文将带你避开所有坑，30分钟上线你的第一个博客。

 为什么选择 Hexo + GitHub Pages？

- 零成本：无需购买服务器，GitHub 免费提供无限流量
- 极速响应：纯静态页面，CDN 加速后秒开
- SEO 友好：预渲染 HTML，百度爬虫可完美收录
- 版本管理：博客即代码，Git 历史记录每一次写作

 三步快速部署

 1. 环境准备（5分钟）

确保本地已安装 Node.js（v18+）和 Git。若未安装，请先前往官网下载对应系统版本。

 2. 初始化 Hexo 项目（10分钟）

```bash
 全局安装脚手架
npm install -g hexo-cli

 初始化博客目录
hexo init my-blog && cd my-blog

 安装依赖并本地预览
npm install && hexo server
```

此时浏览器访问 `http://localhost:4000`，你会看到默认博客主题。

 3. 部署到 GitHub Pages（15分钟）

在 GitHub 创建仓库，命名为 `你的用户名.github.io`。打开项目根目录的 `_config.yml`，修改部署信息：

```yaml
deploy:
  type: git
  repository: https://github.com/你的用户名/你的用户名.github.io.git
  branch: main
```

执行两行命令完成推送：

```bash
npm install hexo-deployer-git --save
hexo clean && hexo deploy
```

等待 3 分钟，访问 `https://你的用户名.github.io`，属于你的博客已上线！

 进阶优化技巧

- 收录提速：在 Google Search Console 和百度站长平台提交站点地图 `/sitemap.xml`
- 主题美化：搜索 `Hexo 主题`，推荐安装 `Next` 或 `Fluid`，功能丰富且响应式支持良好
- 评论系统：接入 `Giscus`，利用 GitHub Discussions 实现免费评论

---

你准备好开始写作了吗？ 如果在部署中遇到任何报错，欢迎在评论区留下你的错误代码，我会逐一解答。关注我，后续将分享更多关于自动化部署、SEO 优化的实战干货。

相关推荐：

https://github.com/riveraevan7367/kwrlsf/blob/main/2027%E5%AE%98%E6%96%B9%E7%9B%98%E7%82%B9%EF%BC%9A%E6%91%A9%E7%99%BB%E5%AE%98%E6%96%B9%E5%BC%80%E6%88%B7_%E9%85%9D%E8%A1%94%E4%BE%A3%E5%AF%90%E9%83%8Afsyxe.md

<img src="https://i.postimg.cc/hj6GxVbz/modeng-00007.png" />

相关推荐：

https://github.com/riveraevan7367/kwrlsf/commit/cef2521672bce5b0e9a56d065a3a0039819aa77b

<img src="https://i.postimg.cc/rmKmKf4B/modeng-00003.png" />
相关推荐：

https://github.com/wangdavid96/psypgl/blob/main/2027%E6%9D%83%E5%A8%81%E6%89%8B%E5%86%8C%EF%BC%9A%E6%91%A9%E7%99%BB%E5%AE%98%E6%96%B9%E5%9C%B0%E5%9D%80_%E7%83%AD%E5%9B%9B%E6%8E%A8%E8%B6%9F%E9%B9%A4ysmtu.md

<img src="https://i.postimg.cc/qRS7n2Xz/modeng-00006.png" />
相关推荐：

https://github.com/wangdavid96/psypgl/commit/e09eabfe475560711e9a7bc51c2dc3f2545e0db5

<img src="https://i.postimg.cc/qv4v8JnJ/modeng-00013.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
