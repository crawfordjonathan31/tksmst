大众娱乐网址【Q-——333307——】大众娱乐网址【 辋芷《888yx●vip》 】
大众娱乐网址【Q-——333307——】大众娱乐网址【 辋芷《888yx●vip》 】

 从零搭建个人博客：GitHub Pages + Hexo 完整教程（2025版）

还在羡慕别人优雅的技术博客？其实你只需要一个 GitHub 账号，就能免费拥有专属博客。本文手把手教你用 Hexo 框架部署到 GitHub Pages，全程零成本、免服务器。

 为什么选择 GitHub Pages + Hexo？

- 完全免费：托管在 GitHub，不限流量
- 极速访问：全球 CDN 加速，国内访问也流畅
- Markdown 写作：专注内容，无需关心排版
- 主题丰富：300+ 主题随意切换，总有一款适合你

 三步搭建专属博客

 第一步：环境准备（5分钟）

1. 安装 [Node.js](https://nodejs.org)（LTS 版本即可）
2. 安装 Git 并配置好全局用户信息

 第二步：初始化 Hexo（10分钟）

```bash
 全局安装 Hexo
npm install -g hexo-cli

 初始化博客项目
hexo init my-blog
cd my-blog
npm install

 本地预览
hexo s
```

访问 `http://localhost:4000` 看到默认博客即成功。

 第三步：部署到 GitHub Pages（10分钟）

1. 创建仓库：`用户名.github.io`（必须同名）
2. 安装部署插件：`npm install hexo-deployer-git --save`
3. 修改 `_config.yml` 配置：

```yaml
deploy:
  type: git
  repo: https://github.com/你的用户名/你的用户名.github.io.git
```

4. 一键部署：

```bash
hexo clean && hexo g && hexo d
```

看到 `Deploy done` 即成功，访问 `https://你的用户名.github.io` 见证奇迹。

 进阶优化：让博客更专业

- 绑定自定义域名：在仓库 Settings 的 Pages 中填写域名，并添加 CNAME 解析
- SEO 优化：安装 `hexo-generator-sitemap` 插件，提交百度站长平台
- 评论系统：集成 Giscus 或 Valine，与读者互动
- 图片优化：使用 `hexo-asset-image` 插件实现本地图片管理

 常见问题排查

- 部署失败：检查仓库名是否与用户名一致，确认 SSH key 已配置
- 样式丢失：清空浏览器缓存，或运行 `hexo clean` 后重新生成
- 访问超时：国内建议配置 CDN 加速（如 Cloudflare）

 开始你的写作之旅

现在你已经拥有了专属博客，接下来就是坚持输出优质内容。建议每周更新 1-2 篇技术笔记或心得总结，持续写作是提升影响力的关键。

遇到问题？欢迎在评论区留言讨论，或搜索更多 Hexo 教程。如果你觉得本文有帮助，点赞、收藏、转发支持一下吧！

你的第一个博客主题准备选哪个？评论区聊聊，我帮你避坑！

相关推荐：

https://github.com/herringjonathan3/cwestb/blob/main/Tr%E1%BB%B1c%20tuy%E1%BA%BFn%20%F0%9F%90%93%EF%BC%9A%E5%A4%A7%E4%BC%97%E5%A8%B1%E4%B9%90%E4%BB%A3%E7%90%86_%E9%93%BA%E5%AD%9F%E8%B5%98%E5%BD%BB%E4%BC%9Ftfyjj.md

<img src="https://i.postimg.cc/jjwm9kFv/dazhong-00003.png" />

相关推荐：

https://github.com/herringjonathan3/cwestb/commit/20782b2f4220ccc3e55a2f0c32d5d7144650b4fb

<img src="https://i.postimg.cc/Rh9YWCZ6/dazhong-00008.png" />
相关推荐：

https://github.com/hilltimothy3744/xgiwkr/blob/main/Tr%E1%BB%B1c%20tuy%E1%BA%BFn%20%F0%9F%90%93%EF%BC%9A%E5%A4%A7%E4%BC%97%E5%A8%B1%E4%B9%90%E4%B8%8B%E8%BD%BD_%E6%B0%90%E8%B0%96%E5%95%A5%E5%95%84%E5%A0%82lmirg.md

<img src="https://i.postimg.cc/dt5f0YMn/dazhong-00014.png" />
相关推荐：

https://github.com/hilltimothy3744/xgiwkr/commit/e36af6d9541a2e1f2b80c4c7420604451ce5e8c6

<img src="https://i.postimg.cc/gjd7xc2z/dazhong-00007.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
