# kaka-cardcrafter 🃏

**卡咔 CardCrafter AI 官方 Agent Skill**——让 WorkBuddy / OpenClaw / Claude Code / Codex 等 AI Agent
直接生成**小红书爆款图文、公众号封面、知识卡片**。输入文字，出可直接发布的成图，无需装任何本地渲染环境。

> 与本地模板类 skill 的区别：卡咔走云端生成管线（远程 MCP / REST API），零本地依赖（不需要
> Node/Playwright），网页端、浏览器插件、Agent 三端同账号同能量，出图失败自动退款。

## 能力

- **小红书爆款图文**：大纲 → 确认 → 多页配图（3~15 页，3:4），支持整稿改大纲、单页重生
- **多规格封面**：一次出公众号横版 2.35:1、3:4、9:16 等平台规格
- **知识卡片**：一段文字 → 自动润色 → 多页卡片，支持风格参考图锁定全套统一风格
- **公版诗词知识库**：节气节日 / 情绪治愈 / 四季风景 / 人生节点四大诗词集，日签类内容一键导入
- **实时数据源**：天气 / 汇率 / 资讯类日签开箱即用（免 Key）
- 出图异步轮询、部分失败自动提示单页重做；能量计费与卡咔网页端同价

## 安装（三选一）

**① WorkBuddy 技能市场**：技能面板搜索「卡咔」或 `kaka-cardcrafter` → 一键安装。

**② ClawHub CLI**：

```bash
clawhub install kaka-cardcrafter
```

**③ 通过 URL 导入**：技能管理 → 添加技能 → 通过 URL 导入 → 填本仓库地址。

## 配置

安装后设置环境变量 `KAKA_API_KEY`（`kc-` 开头）：

1. 打开 **https://www.cardcrafter.cn** 并登录卡咔账号
2. 进入「API 接入」页面 → 点「生成 API Key」（明文只显示一次）
3. `export KAKA_API_KEY=kc-你复制的key`

可选 `KAKA_BASE_URL`（默认 `https://api.cardcrafter.cn`）。

> 也可以不装本技能、直接连卡咔远程 MCP（17 个工具）：
> 插件 → MCP 服务器 → 配置 MCP，端点 `https://api.cardcrafter.cn/mcp`。
> 图文教程：https://www.cardcrafter.cn/platforms/workbuddy

## 使用示例

- 「帮我写一篇三伏天养生茶的小红书图文，6 页」
- 「把这篇读书笔记做成一套小红书图文卡片，5 张，风格统一」
- 「给这篇公众号文章配一张横版封面，标题《……》」
- 「用诗词库生成下周的节气日签，批量 7 张」

## 适用场景

小红书图文组图 · 公众号封面 · 知识卡片 · 读书笔记图文卡片 · 诗词/节气日签 · 金句卡 · 批量风格统一出图

## 链接

- 官网：https://www.cardcrafter.cn
- ClawHub：https://clawhub.com/skills/kaka-cardcrafter
- WorkBuddy 接入教程：https://www.cardcrafter.cn/platforms/workbuddy
- 豆包工作接入教程：https://www.cardcrafter.cn/platforms/doubao
- 完整开放平台 API 文档（skill 版）：https://api.cardcrafter.cn/openapi/skill.md
