大众官方平台【Q-——333307——】大众官方平台【 辋芷《888yx●vip》 】
大众官方平台【Q-——333307——】大众官方平台【 辋芷《888yx●vip》 】

 还在手动部署？GitHub Actions 自动化工作流实战指南，看完就能上手！

兄弟们，是不是每次提交代码后还要手动 SSH 登录服务器拉取更新？或者每天凌晨定闹钟起来跑测试脚本？今天咱不聊虚的，直接聊聊 GitHub Actions 这玩意到底怎么帮你把重复劳动全干掉。

 首先，Actions 是个啥？

简单说，就是 GitHub 给你提供的免费 CI/CD 服务器（虽然有限额，但个人项目完全够用）。你只需要在仓库里建个 `.github/workflows` 文件夹，写个 YAML 配置文件，剩下的触发、跑测试、部署、发通知，它全包了。

核心关键词提前埋伏： `CI/CD`、`自动化部署`、`YAML配置`、`Workflows`、`持续集成`、`DevOps`、`代码推送触发`、`定时任务`、`多环境部署`、`Secrets管理`。

 三步上手，比你想的简单

第一步：建文件
在项目根目录创建 `.github/workflows/deploy.yml` 文件。别怕，就是纯文本。

第二步：写核心配置
一个最基础的流水线长这样：
```yaml
name: 自动部署
on:
  push:
    branches: [ "main" ]
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - name: 安装依赖
        run: npm install
      - name: 跑测试
        run: npm run test
```

第三步：触发
代码推送到 main 分支，Actions 自动开跑。你在仓库的 Actions 标签页能看到实时日志，跑没跑、哪步挂了，全给你列清楚。

 高级玩法：定时任务与密钥管理

如果哪天你想每天凌晨 3 点自动备份数据库，把 `on` 那段换成：
```yaml
on:
  schedule:
    - cron: '0 3   '
```
搞定。至于数据库密码这些敏感信息，千万别写死在代码里。去仓库 Settings -> Secrets and variables -> Actions 里配置 `DB_PASSWORD`，然后在 YAML 里用 `${{ secrets.DB_PASSWORD }}` 引用就行，日志里自动打码。

 踩坑提醒（血泪教训）

1. 缩进必须空格，不能用 Tab，报错能折腾你半小时。
2. Ubuntu 虚拟机环境是全新的，每次跑都要重新装依赖，建议自己写缓存策略。
3. 部署到服务器 需要 SSH 密钥，用 `appleboy/ssh-action@v1.0.0` 这个现成插件，别自己造轮子。

 互动一下

你目前项目里最容易烦躁的重复操作是啥？是部署、测试还是发版？评论区说出来，我挑点赞最高的，下一期专门写个针对性的自动化方案。

觉得有用的话，点个 Star 或者 转发 给你那个还在手动部署的同事。关注我，后续更新不迷路。GitHub Actions 这波车，你不上，真亏了。

相关推荐：

https://github.com/wangdavid96/psypgl/blob/main/C%E1%BB%91c%20Games%20%F0%9F%A5%8A%EF%BC%9A%E5%A4%A7%E4%BC%97%E7%BD%91%E5%9D%80%E5%BC%80%E6%88%B7_%E7%8A%B9%E5%8F%B8%E5%92%BD%E6%80%82%E7%9B%B4edqrq.md

<img src="https://i.postimg.cc/1XHjwx8W/dazhong-00011.png" />

相关推荐：

https://github.com/wangdavid96/psypgl/commit/2f26380d5c1a2eff4edd0634a686dbb77fdc753c

<img src="https://i.postimg.cc/2ywKhp1b/dazhong-00009.png" />
相关推荐：

https://github.com/herringjonathan3/cwestb/blob/main/Th%E1%BB%83%20thao%20%E2%9A%BD%EF%B8%8F%EF%BC%9A%E5%A4%A7%E4%BC%97%E7%BD%91%E5%9D%80%E7%99%BB%E5%BD%95_%E4%B9%A9%E8%B7%AF%E7%99%BD%E6%97%81%E8%B1%AAgbxaq.md

<img src="https://i.postimg.cc/gjd7xc2z/dazhong-00007.png" />
相关推荐：

https://github.com/herringjonathan3/cwestb/commit/e07bbeaa1438bbc2aec2cc687ab2dfd46367a7e4

<img src="https://i.postimg.cc/jjwm9kFv/dazhong-00003.png" />

资讯来源：新华网、人民网、央视新闻、中新网、凤凰网、澎湃新闻、界面新闻、新浪新闻、搜狐网、财新网、观察者网、第一财经等主流平台，以独树一帜的观察视角与扎实的深度报道能力，在资讯领域收获广泛关注。
