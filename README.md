<h1 align="center">Hoodas</h1>

<p align="center">
  <b>教育行业从业者 · 独立开发者</b><br>
  <sub>白天经营教培机构，晚上给自己写工具。<br>所有软件都是先解决自己的问题，再开源出来。</sub>
</p>

<p align="center">
  <a href="#项目">项目</a> ·
  <a href="#为什么开源">为什么开源</a> ·
  <a href="#联系与合作">联系与合作</a>
</p>

---

## 项目

### 星课 StarClass — 小型教培机构的整套管理系统

> **一次部署，长期使用。不收年费，不限人数，学员数据留在你自己的机器里。**

招生、排课、考勤、家校沟通、销售续费、薪资结算一套全包。Vue3 + Express + SQLite，不依赖任何云服务，一条命令跑起来。按生产标准写：**34 套回归测试**覆盖支付幂等、退款回收、越权与审计留痕，Node 18/20/22 三版本 CI 全绿。

| | |
|---|---|
| 🖥️ Web 后台 | 23 个页面视图 · 深浅色主题 · 手机号+密码登录 |
| 📱 小程序扩展 | 家长 / 教练 / 管理三端（可选，商业授权） |
| 🧱 部署 | `bash deploy.sh` 一键，或 Docker + 自动 HTTPS |
| 📖 文档 | [使用手册](https://github.com/Hoodas101/starclass/blob/main/使用手册.md) · [部署上线说明](https://github.com/Hoodas101/starclass/blob/main/部署上线说明.md) · [FAQ](https://github.com/Hoodas101/starclass/blob/main/docs/常见问题FAQ.md) |

[**查看项目**](https://github.com/Hoodas101/starclass)

---

### LidKeep — 关掉屏幕，机器照常跑

> **只关背光，显示器从不进入睡眠。远程端看到的还是真实画面。**

macOS 把「屏幕灭」和「机器睡」绑成了一件事，LidKeep 把它们拆开：屏幕全黑省电，机器继续跑。远程桌面不掉线，下载和构建不受影响，SSH 一直在，合盖也一样。

一行安装 · 零第三方依赖 · 无账号无遥测 · MIT 开源 · 中文文档齐全。

| | |
|---|---|
| ⌨️ 热键 | ⌃⌥⌘B 一键熄屏 / 恢复 |
| 💻 CLI | `lidkeep off` / `on` / `status` / `doctor` / `plan` |
| 🔌 电源计划 | 插电与电池分别配置，拔电源自动切换 |
| 📖 文档 | [详细说明](https://github.com/Hoodas101/lidkeep/blob/main/docs/DETAILS.zh-CN.md) · [配置项](https://github.com/Hoodas101/lidkeep/blob/main/docs/CONFIG.md) · [场景配方](https://github.com/Hoodas101/lidkeep/blob/main/docs/COOKBOOK.md) |

[**Releases / 下载**](https://github.com/Hoodas101/lidkeep/releases/latest) · [**中文说明**](https://github.com/Hoodas101/lidkeep/blob/main/README.zh-CN.md)

---

## 为什么开源

起点都是「我自己需要」：机构管不过来就写 StarClass，远程用的 Mac 一熄屏就断线就写 LidKeep。既然要写，就按能长期用、能交给别人用的标准写：CI、回归测试、变更日志和排障文档，都是我自己每天在用的东西。

---

## 联系与合作

- **StarClass 小程序 · 部署服务 · 机构定制**，欢迎在 [StarClass Issues](https://github.com/Hoodas101/starclass/issues) 留言咨询（中文即可，首次咨询免费评估是否适合）
- 发现问题请开 Issue，每个报告我都会看，多数修复在几天内落地
- 项目帮到你了？点个 Star 是成本最低、帮助最大的支持方式；想再进一步可以走 [GitHub Sponsors](https://github.com/sponsors/Hoodas101)

<p align="center">
  <sub>
    如果你也在教育行业写代码，或者想给自己的机构做一套系统，随时聊聊。<br>
    StarClass · LidKeep
  </sub>
</p>
