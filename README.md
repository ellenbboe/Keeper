<!--
 * @Author: Weidows
 * @Date: 2020-11-28 17:36:36
 * @LastEditors: Weidows
 * @LastEditTime: 2021-10-10 15:10:54
 * @FilePath: \Keeper\README.md
 * @Description:
-->

<h1 align="center">

- ## 🌈Keeper

基于 [`GitHub-Action`](./.github/workflows/daily.yml) 的定时任务集合.

</h1>

# Feature

- [x] 每日 push `刷绿 profile 格子`, 预览: [GitHub](https://github.com/Weidows) / [Gitee](https://gitee.com/Weidows)
- [x] 每日访问唤醒休眠的 LeanCloud 评论后台 (也可以是其他地址)
- [x] 每日获取`必应壁纸`,存储在[Bing](./Bing/)里面.
- [x] 每次执行任务会把 Log 记录在 `Tasks.log` 中,可自定义信息.
- [ ] 每日同步 github 仓库到 gitee.

![分割线](https://cdn.jsdelivr.net/gh/Weidows/Images/img/divider.png)

# Usage

- ## 首先声明

  - Fork 本项目不会产生 GitHub 刷绿效果! (Fork 项目的提交不被计数)
  - 给个 Star 呗, 还会更新呢!
  - 技术性探索,主旨非作弊行为,默认为非开启状态.

- [`下载/clone`](https://github.com/Weidows/Keeper/releases)本项目,自己新建一个仓库或者把本仓库文件复制到目标仓库`根目录`.

![分割线](https://cdn.jsdelivr.net/gh/Weidows/Images/img/divider.png)

# config-[secret](https://github.com/Weidows-projects/Keeper/settings/secrets/actions)

| secret-name |                                                                               value (不会泄露,未填的项不会启用)                                                                               |
| :---------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| PUSH_EMAIL  |                                                                         github 推送邮箱 (默认使用 Github-action[bot])                                                                         |
|     URL     |                                                    需要唤醒的地址,支持多个如 `https://weidows.avosapps.us/comments https://www.baidu.com`                                                     |
|  GITEE_RSA  | 私钥文件内容; 公钥复制到 [用户设置](https://gitee.com/profile/sshkeys); 如何生成秘钥可以查看 [这篇文章](https://weidows.github.io/post/experience/SSH); 需要提前在 gitee 创建同名同邮箱的仓库 |
| GITEE_TOKEN |                                            用于镜像时自动创建不存在的仓库,Gitee 可以在[这里](https://gitee.com/profile/personal_access_tokens)找到                                            |

---

- 最后进入你的仓库里`enable Action`, 手动 star 或者东八区早八点会自动执行.

![分割线](https://cdn.jsdelivr.net/gh/Weidows/Images/img/divider.png)

# 借鉴

> [justjavac/auto-green](https://github.com/justjavac/auto-green) \
> [mstf/bingdownload](https://gitee.com/mstf/bingdownload) \
> [Yikun/hub-mirror-action](https://github.com/Yikun/hub-mirror-action/)
