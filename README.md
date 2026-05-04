# 小宏单词 (XiaoHong Words)

一个极简、高效的英文单词记忆工具，基于认知科学原理设计。

[在线体验](https://ycc-ong.github.io/xiaohong-words/)

## ✨ 功能

- **翻转卡片学习** — 3D 翻转查看词义，结合词源故事 + 联想记忆法
- **听音拼写** — 听发音打出单词，强化拼写记忆
- **选择题测验** — 多选一考验理解
- **速记闪卡** — 快速闪过，双侧按钮秒判断
- **艾宾浩斯遗忘曲线** — 5 级间隔自动调度复习（0.5分钟 / 3分钟 / 8分钟 / 20分钟 / 掌握）
- **成就系统** — 8 种徽章激励
- **XP 经验值 + 连续打卡** — 正向反馈闭环
- **番茄钟** — 专注计时器
- **文件导入** — 支持 .txt / .csv / .json 三种格式，拖拽/粘贴/选文件
- **localStorage 持久化** — 数据存本地，打开就恢复进度

## 🧠 设计原理

基于多项记忆科学实证研究：

| 原理 | 应用 |
|------|------|
| **主动回忆** (Active Recall) | 听音拼写、测验模式 |
| **双重编码** (Dual Coding) | 翻转卡片 + 发音 + 例句多感官刺激 |
| **生成效应** (Generation Effect) | 拼写模式主动生成答案 |
| **交错练习** (Interleaving) | 多模式切换训练 |
| **间隔重复** (Spaced Repetition) | 艾宾浩斯 5 级调度 |

## 🚀 使用方法

1. 直接在浏览器打开 `vocab.html`
2. 或部署到任意静态托管（GitHub Pages / Netlify / Vercel）

### 导入自己的词库

支持三种格式：

**txt**（单词 - 释义）：
```
abandon - 放弃；抛弃
brilliant - 明亮的；杰出的
```

**csv**：
```
word,meaning
apple,苹果
computer,电脑
```

**json**：
```json
[{"w": "hello", "m": "你好"}, {"w": "world", "m": "世界"}]
```

## 🛠 技术栈

- 纯 HTML + CSS + JavaScript，零依赖
- Web Speech API 实现 TTS 发音
- localStorage 数据持久化
- SVG 进度环

## 📂 文件结构

```
├── index.html        # 主应用（GitHub Pages 入口）
├── vocab.html        # 同上，备用名称
├── test-words.txt   # 测试用词库样本
├── README.md        # 项目说明
└── .gitignore       # Git 忽略规则
```

## 📄 License

MIT
