# 🌅 开盘前全球情报简报生成器

<p align="center">
  <strong>每日早间全球市场要闻 · 一键生成专业 HTML 简报</strong>
  <br>
  自动聚合隔夜美股、亚太早盘、全球资产、A 股盘面深度等八大模块，
  输出黑底科技风交互式 HTML 简报（完整版 + 摘要卡双件套）。
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="version 1.0.0"/>
  <img src="https://img.shields.io/badge/license-MIT-green" alt="license MIT"/>
  <img src="https://img.shields.io/badge/category-finance-orange" alt="category finance"/>
  <img src="https://img.shields.io/badge/color%20scheme-红涨绿跌-red" alt="A股红涨绿跌"/>
</p>

---

## 📋 功能概览

每个交易日开盘前，自动生成一份**专业级全球市场情报简报**，覆盖全球主要市场的核心动态：

### 完整增强版（八章结构）

| 模块 | 内容 |
|------|------|
| ① **一屏核心结论** | 当日最关键的市场信号与判断，一眼速览 |
| ② **隔夜美股全天** | 道指/标普/纳指收盘 + 11 行业板块强弱表 |
| ③ **全球资产温度计** | 原油/黄金/美元/美债/人民币/VIX + A 股映射影响 |
| ④ **外围映射与期指** | 富时 A50 / 恒生期货 / 中概金龙指数 |
| ⑤ **昨夜预判对账** | 前日预判 vs 实际走势，量化命中率 |
| ⑥ **日韩早盘** | 日经 225 / KOSPI 早盘涨跌幅及领涨权重 |
| ⑦ **隔夜全球新闻** | 重大宏观事件 + A 股关联影响分析 |
| ⑧ **A 股盘面深度** | 指数/市场宽度/资金流 + 当日预判 & 板块温度计 |

### 摘要卡（浓缩版）

同风格 1-2 屏浓缩，去冗余只留高价值信息，适合快速扫读。

## 🚀 快速开始

### 作为 Tango AI Agent Skill 使用

在 Tango 平台中，直接通过自然语言触发：

```
# 生成今日简报
生成开盘前全球要闻简报

# 指定日期
生成昨天的盘前情报

# 晨间速览
早间要闻摘要卡
```

### 独立使用

```bash
git clone https://github.com/benstartnow/premarket-global-brief.git
cd premarket-global-brief
```

## 🏗️ 项目结构

```
premarket-global-brief/
├── SKILL.md                        # Skill 核心定义 — 执行流程、数据源、合规红线
├── assets/                         # 模板资源（预留）
├── references/                     # HTML 模板参考
│   ├── full_version.html           # 完整增强版模板（黑底科技风）
│   └── summary_version.html        # 摘要卡模板（同风格 1-2 屏）
└── scripts/                        # 辅助脚本（预留）
```

## 🔧 技术栈

| 组件 | 用途 |
|------|------|
| **HTML + CSS** | 简报渲染（黑底 `--bg: #0b0f14` / 科技青 `--accent: #2dd4bf` / 金色标题 `--gold: #e6b450`） |
| **WebSearch** | 实时数据采集（美股收盘、亚太早盘、宏观新闻） |
| **NeoData / 东方财富 / CNBC** | 市场数据来源 |

## 📖 执行流程

1. **联网取数** — 并行搜索美股收盘、亚太早盘、A 股前收、全球资产、宏观要闻
2. **生成完整增强版** — 八章结构 HTML，遵循红涨绿跌（A 股习惯）配色
3. **生成摘要卡** — 同风格 1-2 屏浓缩，去冗余保核心
4. **双件交付** — 同时输出完整版 + 摘要卡

## ⚙️ 数据来源

- **美股**：CNBC / 新浪财经
- **亚太**：日经 / 韩国交易所
- **A 股**：东方财富 / 新浪财经
- **全球资产**：Wind / 路透
- **宏观新闻**：主流财经媒体

## ⚠️ 合规红线

- ❌ 不出现"推荐/买入/看好/目标/建仓"等引导词
- ❌ 不引导私信代码、加群、跟车
- ✅ 点位/区间一律标注"情绪参考，非精确预测"
- ✅ 必须带"不荐股、不构成投资建议"声明

## 📄 License

本项目基于 MIT License 开源 — 详见 [LICENSE](LICENSE) 文件。

---

<p align="center">
  <sub>Made by <a href="https://github.com/benstartnow">@benstartnow</a></sub>
</p>
