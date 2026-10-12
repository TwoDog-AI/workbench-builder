# 图标

工作台只用 `assets/icons.svg` 里的图标。它们来自 Lucide（ISC 协议），已经挑好了工作台常用的 70 个，不需要联网加载。

## 用法

1. 打开 `assets/icons.svg`，只把这次页面用到的 `<symbol>` 复制进页面 `<body>` 开头的一个隐藏 `<svg style="display:none">` 里。不要整份粘贴。
2. 在需要的位置这样引用：

```html
<svg class="icon" aria-hidden="true"><use href="#i-calendar"/></svg>
```

3. 尺寸和线宽由 `themes.css` 的 `.icon` 统一控制（20px、线宽 1.75），紧凑处加 `icon-sm`（16px）。颜色自动跟随文字颜色，需要变色就改父元素的 `color`。
4. 不要给单个图标写死 `width`、`stroke-width` 或颜色。

## 无障碍

- 图标旁边有文字时，图标加 `aria-hidden="true"`。
- 只有图标的按钮，按钮本身要有 `aria-label` 和 `title`：

```html
<button class="icon-btn" aria-label="删除这条" title="删除这条">
  <svg class="icon" aria-hidden="true"><use href="#i-trash"/></svg>
</button>
```

- 按钮可点击区域至少 32×32px（手机上 44×44px），图标本身小没关系，用内边距撑大。

## 原则

- 不用 emoji、Unicode 符号（✓ ★ → ● ☐）代替图标。
- 图标帮助识别和操作，不是装饰。模块标题前不必都放图标；放了就整页都放，保持一致。
- 同一个意思全页用同一个图标。
- 这里没有合适的，宁可不用图标、只用文字，也不要临时手画 SVG 或混用其他图标库。

## 图标清单

| id | 用途 |
|---|---|
| `i-plus` | 添加 |
| `i-minus` | 减少 |
| `i-check` | 完成、勾选 |
| `i-circle-check` | 已完成状态 |
| `i-square` | 未勾选的待办 |
| `i-square-check-big` | 已勾选的待办 |
| `i-trash` | 删除 |
| `i-pencil` | 编辑 |
| `i-square-pen` | 写新内容 |
| `i-x` | 关闭、移除 |
| `i-search` | 搜索 |
| `i-calendar` | 日期、日程 |
| `i-calendar-days` | 周视图、月视图 |
| `i-clock` | 时间 |
| `i-timer` | 计时、专注 |
| `i-alarm-clock` | 提醒、闹钟 |
| `i-bell` | 通知 |
| `i-sticky-note` | 随手记 |
| `i-notebook-pen` | 笔记、日记 |
| `i-book-open` | 阅读、学习 |
| `i-file-text` | 文档 |
| `i-folder` | 分类、文件夹 |
| `i-archive` | 归档 |
| `i-tag` | 标签 |
| `i-link` | 链接 |
| `i-external-link` | 在新窗口打开 |
| `i-globe` | 网站 |
| `i-star` | 收藏 |
| `i-pin` | 置顶 |
| `i-flag` | 重要、截止 |
| `i-target` | 目标 |
| `i-inbox` | 收集箱 |
| `i-list-todo` | 待办清单 |
| `i-list-checks` | 检查清单 |
| `i-layout-dashboard` | 工作台总览 |
| `i-sparkles` | AI 生成的内容 |
| `i-bot` | AI 助手 |
| `i-message-circle` | 对话 |
| `i-send` | 发送 |
| `i-wallet` | 钱包、预算 |
| `i-receipt` | 账单、报销 |
| `i-chart-column` | 统计 |
| `i-trending-up` | 上升 |
| `i-trending-down` | 下降 |
| `i-lightbulb` | 灵感、想法 |
| `i-coffee` | 休息 |
| `i-briefcase` | 工作、客户 |
| `i-graduation-cap` | 课程、学生 |
| `i-shopping-cart` | 购物清单 |
| `i-utensils` | 吃饭、菜谱 |
| `i-baby` | 孩子 |
| `i-users` | 家人、团队 |
| `i-user` | 个人 |
| `i-house` | 家 |
| `i-heart` | 健康、喜欢 |
| `i-repeat` | 重复、习惯 |
| `i-mail` | 邮件 |
| `i-phone` | 电话 |
| `i-sun` | 浅色模式 |
| `i-moon` | 深色模式 |
| `i-settings` | 设置 |
| `i-sliders-horizontal` | 调整 |
| `i-chevron-down` | 展开 |
| `i-chevron-right` | 进入、收起 |
| `i-grip-vertical` | 拖动排序 |
| `i-ellipsis` | 更多操作 |
| `i-copy` | 复制 |
| `i-refresh-cw` | 刷新、重试 |
| `i-play` | 开始 |
| `i-pause` | 暂停 |