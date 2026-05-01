# AnimeVault 🎬  
**智能动漫推荐与内容管理平台**

[![Project Status](https://img.shields.io/badge/status-active-brightgreen)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)]()
[![Powered by MiMo](https://img.shields.io/badge/AI-MiMo%202.5%20Pro-blue)]()

AnimeVault 是一个为动漫爱好者打造的纯净追番工具，专注于解决当前免费动漫平台的**广告泛滥、信息碎片化、推荐低质**三大痛点。通过集成 **MiMo 2.5 Pro** 的强大推理与生成能力，为用户提供高度个性化的番剧推荐与自动化的内容管理。

---

## ✨ 核心特性

- **🧠 智能语义推荐**  
  基于 MiMo 的长链推理，分析用户观看历史中的叙事风格、节奏偏好，实现跨类型精准推荐。  
  示例：看完《葬送的芙莉莲》，不仅推荐《无职转生》，还会推荐《三月的狮子》《虫师》等气质相似的作品。

- **📋 自动化内容管理**  
  调用 MiMo API 自动生成番剧摘要、标签体系（如 #慢节奏 #情感细腻 #公路片），并实时审核内容合规性。

- **🔌 数据实时同步**  
  通过 Jikan API 拉取 MyAnimeList 官方元数据，保证评分、声优、播出时间的准确性。

- **🎨 纯净用户体验**  
  无侵入式广告，界面遵循 Material Design 3，React + Tailwind CSS 构建，流畅响应式。

---

## 🧱 技术栈

| 层         | 技术                            |
|------------|---------------------------------|
| 前端       | React 18, Tailwind CSS, Radix UI |
| 后端       | Node.js, Express                |
| AI 服务    | MiMo-V2.5-Pro (推荐 + 生成)      |
| 数据源     | Jikan API v4 (MAL)              |
| 开发环境   | VS Code + Cline 插件 + MiMo API  |

---

## 🚀 快速开始（本地开发）

> 注意：项目目前处于架构阶段，以下流程即将可用。

```bash
# 1. 克隆仓库
git clone https://github.com/shengming8/AnimeVault.git
cd AnimeVault
Initial commit: add project README
# 2. 安装依赖
npm install

# 3. 配置环境变量
cp .env.example .env
# 打开 .env 文件，填入 MIMO_API_KEY=你的key

# 4. 启动开发服务器
npm run dev
详细 API 文档见 MiMo 开放平台
📂 项目结构（规划中）
AnimeVault/
├── public/               # 静态资源
├── src/
│   ├── components/       # UI 组件
│   ├── hooks/            # 自定义 hooks
│   ├── services/         # API 调用（MiMo, Jikan）
│   ├── utils/            # 工具函数
│   └── App.tsx
├── server/               # 后端
│   ├── routes/
│   ├── controllers/
│   └── services/
├── .env.example          # 环境变量模板
├── .gitignore
├── package.json
└── README.md
🤝 贡献
本项目正在积极开发中，欢迎 Star 和 Fork。由于使用了 MiMo API 的 Token 免费额度，我们将在额度正式到账后开放部分测试接口。

📄 许可证
MIT License.
