# 个人工作台 skill

让不熟悉 AI 的用户说一句“创建工作台”，通过一问一答生成一个属于自己的工作台网页。生成的是单个 HTML 文件，双击就能用，数据保存在浏览器里，可导出导入。不需要 Python、不需要联网、不依赖其他 skill。

## 安装

把整个 `workbench-builder` 文件夹放进 agent 的 skills 目录即可（例如 Claude Code 的 `~/.claude/skills/`）。

## 结构

```
workbench-builder/
├── SKILL.md               主流程：创建、修改、交付
├── references/
│   ├── interview.md       问答流程、问题库、按身份的默认搭配
│   ├── modules.md         配置格式和 13 种模块
│   ├── themes.md          六套主题和字体加载策略
│   ├── checklist.md       生成后自检
│   ├── design.md          设计规范（调整视觉时用）
│   └── icons.md           图标用法和清单
├── assets/
│   ├── workbench.html     工作台模板（内嵌了主题、图标和全部模块代码）
│   ├── themes.css         主题源文件
│   ├── icons.svg          69 个 Lucide 图标
│   └── theme-preview.html 主题预览页
├── LICENSES/              上游许可证原文
└── NOTICE.md              第三方声明
```

## 工作方式

模型只负责“问清楚、选模块、填内容”，不写界面代码：问答结果写成一段配置 JSON，放进 `workbench.html` 的副本里就完成了。这样不同模型、不同 agent 生成的工作台质量都稳定。

## 维护

`workbench.html` 内嵌了 `themes.css` 和 `icons.svg` 的内容。修改主题或图标时，记得把模板里对应的部分同步更新。

## 模块

今天要做的事、今天最重要的一件事、这周的安排、进行中的项目、随手记、常用网站、每天坚持、收支记录、倒数日、目标、想看的书和课、常用 AI 指令、专注计时。
