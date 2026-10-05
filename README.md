<h1 align="center">Hoodas 🖋️</h1>

<p align="center">
  <b>教育行业从业者 · 独立开发者</b><br>
  <sub>白天经营教培机构，晚上给自己写工具。<br>所有软件都是先解决自己的问题，再开源出来。</sub>
</p>

<p align="center">
  <a href="#-项目">项目</a> ·
  <a href="#-为什么开源">为什么开源</a> ·
  <a href="#-联系与合作">联系与合作</a>
</p>

---

## 🔧 项目

### 星课 StarClass — 给小型教培机构的一套完整管理系统

> **一次部署，长期使用。不年费、不限人数、学员数据留在你自己的机器里。**

招生、排课、考勤、家校沟通、销售、续费、薪资结算，一套系统全包。Vue3 + Express + SQLite，零云服务依赖，一条命令跑起来。

这不是「技术 demo」，是按生产标准写的：**34 套自动化回归测试**（覆盖支付幂等、退款回收、跨角色越权、审计留痕、口径一致性），CI 在 Node 18/20/22 三个版本全绿，含部署前自动备份与健康检查。

| | |
|---|---|
| 🖥️ Web 管理后台 | 23 个页面视图 · 深浅色主题 · 手机号+密码登录 |
| 📱 可选小程序扩展 | 家长 / 教练 / 管理三端（41 页，商业授权） |
| 🧱 部署方式 | `bash deploy.sh` 一键（本机）或 Docker + 自动 HTTPS（服务器） |
| 📖 文档 | [使用手册](https://github.com/Hoodas101/starclass/blob/main/使用手册.md) · [部署上线说明](https://github.com/Hoodas101/starclass/blob/main/部署上线说明.md) · [FAQ](https://github.com/Hoodas101/starclass/blob/main/docs/常见问题FAQ.md) |

`git clone https://github.com/Hoodas101/starclass.git && cd starclass && bash deploy.sh`

👉 [**查看项目**](https://github.com/Hoodas101/starclass)

---

### LidKeep — 关掉屏幕，但别让 Mac 睡着

> **只切背光，不进入显示器睡眠 —— 所以远程桌面看到的永远是真实画面，而不是黑屏。**

macOS 把「熄屏」和「系统睡眠」绑在一起。LidKeep 把它们拆开：屏幕全黑省电，但机器继续跑 —— 远程桌面不断线、下载不断、构建不断、SSH 一直可用，合盖也能继续。

一行安装 · 零第三方依赖 · 无账号无遥测 · MIT 开源 · 中文文档齐全。

`curl -fsSL https://raw.githubusercontent.com/Hoodas101/lidkeep/main/install-remote.sh | bash`

| | |
|---|---|
| ⌨️ 热键 | ⌃⌥⌘B 一键熄屏 / 恢复 |
| 💻 CLI | `lidkeep off` / `on` / `status` / `doctor` / `plan` |
| 🔌 电源计划 | 插电与电池分别配置，拔电源自动切换（同 Windows 电源选项模型） |
| 📖 文档 | [详细说明](https://github.com/Hoodas101/lidkeep/blob/main/docs/DETAILS.md) · [配置项](https://github.com/Hoodas101/lidkeep/blob/main/docs/CONFIG.md) · [场景配方](https://github.com/Hoodas101/lidkeep/blob/main/docs/COOKBOOK.md) |

👉 [**Releases / 下载**](https://github.com/Hoodas101/lidkeep/releases/latest) · [**中文说明**](https://github.com/Hoodas101/lidkeep/blob/main/README.zh-CN.md)

---

### 给 AI Agent 的两套「思考质量」skill

> 让 AI 不只是回答，而是**先检查推理、再给结论**。

| Skill | 做什么 | 已有内容 |
|---|---|---|
| [**thinking-models**](https://github.com/Hoodas101/thinking-models) | 分析工具箱：该怎么做更好 | 66 个思维模型 + 分级介入（L0–L3）+ 苏格拉底引导模式 |
| [**bias-correction**](https://github.com/Hoodas101/bias-correction) | 防错护栏：哪里会出错 | 39 个认知偏误 + 双通道触发 + 元层自检 |

两套编号互通（如沉没成本 = TM#1 = BC#29），可单用也可组合。跨平台：Claude Code / Cursor / Codex / Cline / Continue。

**它们对「模型证据强度」逐条标注**：25 个学术共识 / 9 个实证支持 / 14 个经验总结 / 6 个隐喻借用 / 2 个有争议 —— 越听起来深刻的模型往往证据越薄，这一点我们明说。

```bash
curl -fsSL https://raw.githubusercontent.com/Hoodas101/thinking-models/main/install.sh | bash
curl -fsSL https://raw.githubusercontent.com/Hoodas101/bias-correction/main/install.sh | bash
```

---

## 💡 为什么开源

我做的每一个项目，起点都是「我自己需要」：机构管不过来 → 写 StarClass；远程用的 Mac 一熄屏就断线 → 写 LidKeep；AI 回答看着对但经不起追问 → 写思维模型 skill。

既然要写，就按能长期用、能交给别人用的标准写。所以这些仓库里有 CI、有回归测试、有变更日志、有排障文档 —— 这不是给面试官看的装饰，是因为我自己每天在用。

---

## 📮 联系与合作

- **StarClass 三端小程序 · 部署服务 · 机构定制** —— 欢迎在 [StarClass Issues](https://github.com/Hoodas101/starclass/issues) 留言咨询（中文即可，首次咨询免费评估是否适合）
- 发现问题请开 Issue，**每个报告我都会看**，多数修复在几天内落地
- 项目帮到你了？点个 ⭐ 是成本最低、帮助最大的支持方式

<p align="center">
  <sub>
    如果你也在教育行业写代码，或者想给自己的机构做一套系统 —— 随时聊聊。<br>
    StarClass · LidKeep · thinking-models · bias-correction
  </sub>
</p>
