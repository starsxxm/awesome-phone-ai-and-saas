# 从 GitHub 项目规律反推产品机会（Coomi 推理笔记 · 持续更新）

> 方法：不追热点词，找"重复出现的结构性需求"。凡是我们自己真实需要过的需求，欧美用户大概率也需要——这就是 PMF 的土办法。

## 一、观察到的结构性规律（基于本轮爬取）

1. **"监控某个东西，变了就通知我"是超级模式**
   - changedetection.io（网页变化检测，~25k★）、各种 stock/price/deal monitor、uptime monitor 全都在涨
   - 咱们的 ghim（库存监控站）就是同一个模式的具体实例——方向对了
   - 推论：这个模式可以套无数垂直场景：职位刷新、签证位、二手件、票务、Game server 状态、竞品价格
2. ** boilerplate 生意本身就是一个品类**：SaaS starter、Chrome extension+Stripe 脚手架都有人卖钱。"帮开发者省第一周"成立
3. **indie hacker 资料聚合长盛**：awesome-indiehackers 582+ 相关仓库——引流内容有真实受众

## 二、推理出的产品机会（按可信度排序）

### 机会 1：垂直监控 SaaS（ghim 的泛化）★★★★★
- 已验证：changedetection.io 证明付费意愿；ghim 已有代码底座（订阅→审核→抓取→TG/Email/Discord/Webhook 通知）
- 差异化打法：不做通用"网页变化"（红海），做**某个具体人群的"到货/放位"监控**，比如：驾照路考位、破服务器报价、PS5 补货这类。MVP 成本几乎为零（ghim 换抓取目标即可）
- 关键：选一个欧美有线下焦虑的场景，SEO 词很好抢

### 机会 2：手机端"自动化任务"订阅制 ★★★☆☆
- DailyPilot 本身可商业化：自动每日任务对欧美放置玩家是真金白银的痛点
- 风险：游戏厂商风控、Google Play 政策——适合官网直发 APK（Obtainium 模式证明分发可行）
- 前置条件：先跑通真机验证

### 机会 3："给非程序员的自动化"轻工具 ★★★☆☆
- 观察：n8n/Zapier 类项目长盛，但欧美大量小商家只用 TG/Discord
- 产品：把 ghim 的"订阅→抓取→通知"管道包装成"给小商家的 TG 机器人 SaaS"（库存播报、订单通知、竞品盯梢），$5-15/月
- 底座复用：saas-mvp（额度/计费/通知体系全部现成）

### 机会 4：先不做的（诚实记录）
- 通用 AI wrapper、又一个 boilerplate、又一个 changedetection——红海且无差异化

## 三、下一步爬取计划（Loop 式持续）
- [ ] indie hacker 收入验证类仓库（open startup），学他们的定价页
- [ ] Product Hunt 常客的 GitHub（看他们最近在做什么）
- [ ] 按 ghim 的目标人群搜（deals/stock/alert 类）找竞品定价
- 更新规则：每轮爬取后增量追加到本文件，不重写
