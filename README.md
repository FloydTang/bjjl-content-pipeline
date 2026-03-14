# bjjl-content-pipeline 📝⚡

> 半斤九两舰队公众号文章生产流水线 v3.5 — 完整流程：采集 → 标记 → 分发 → 展示 → 决策 → 撰写 → 审稿 → 发布

---

## ✨ 特性

- **双轨搜索策略**：Tavily AI 搜索 + RSS 采集，双管齐下获取选题
- **五维评分系统**：外贸相关性/AI相关性/TikTok相关性/可操作性/时效性
- **多角色协作**：Vector（采集）、九两（决策）、Cypher（撰写）、Echo（发布）
- **自动动作表**：支持"关注选题池"/"关注创作间"自动触发
- **多平台发布**：公众号/知乎/LinkedIn 一键适配发布

## 🎯 价值与意义

- 解决选题效率低下问题：AI 自动采集评分，只推荐高价值选题
- 标准化内容生产流程：6 阶段闭环，角色分工明确
- 降低人工重复劳动：自动同步 GitHub、自动发布

## 🚀 快速开始

### 1. 克隆项目

```bash
git clone https://github.com/FloydTang/bjjl-content-pipeline.git
cd bjjl-content-pipeline
```

### 2. 安装依赖

```bash
pip install -r requirements.txt
```

### 3. 配置环境

```bash
# 配置 Tavily API Key
export TAVILY_API_KEY="tvly-xxx"

# 配置 Discord 账号（Vector/Mars/Cypher/Echo）
```

### 4. 运行

```bash
# Vector: 每日采集
python3 rss_collector.py

# Mars: 检测 👍 并触发后续流程
```

---

## 📂 项目结构

```
bjjl-content-pipeline/
├── SKILL.md              # Skill 定义文档（完整流程说明）
├── README.md             # 项目介绍
├── rss_collector.py      # RSS 采集脚本
└── requirements.txt     # Python 依赖
```

---

## ⚙️ 配置参数

| 参数 | 说明 | 默认值 |
|------|------|--------|
| TAVILY_API_KEY | Tavily 搜索 API | （必填） |
| RSS_SOURCES | RSS 源列表 | 10 个核心源 |
| DISCORD_CHANNELS | 频道映射 | 选题池/创作间 |

---

## 🤝 贡献

欢迎提交 Issue 和 PR！

---

## 📄 许可证

MIT License

---

## 📞 联系

- 创始人：汤九两
- 公司：半斤九两科技

---

## 📋 版本历史

| 版本 | 日期 | 更新内容 |
|------|------|----------|
| v3.5 | 2026-03-14 | 触发入口统一为#内容生产线、新增自动动作表、账号发送规范、子代理调用修正 |
| v3.4 | 2026-03-13 | 自动评分算法优化 |
| v3.3 | 2026-03-13 | 多平台发布支持 |

---

**Version**: 3.5  
**Last Updated**: 2026-03-14
