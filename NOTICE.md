# 第三方声明

本 skill 的设计规范整合并改写了以下开源项目的内容。原许可证全文见 `LICENSES/` 文件夹。

## frontend-design（Anthropic）

- 来源：Anthropic 官方 skills 中的 frontend-design
- 许可证：Apache License 2.0（`LICENSES/frontend-design-Apache-2.0.txt`）
- 使用方式：`references/design.md` 中关于“从使用者和场景出发做设计”“排版层次”“动效克制”“界面文案”的原则，以及常见生成式设计特征的识别，参考了该 skill。
- 修改说明：内容已用中文重写，并针对个人工作台场景和中文排版做了调整与补充，非原文翻译。

## Impeccable（Paul Bakaus）

- 来源：https://github.com/pbakaus/impeccable
- 许可证：Apache License 2.0（`LICENSES/impeccable-Apache-2.0.txt`）
- 使用方式：`references/design.md` 中“主题只贡献字体、配色、密度和一个标志性细节，控件保持标准”的思路参考了其 Operate 模式说明；`references/checklist.md` 中的质量底线和应避免的做法参考了其 craft-floor 规则。
- 修改说明：内容已用中文重写并精简，去掉了对其命令行工具和检测引擎的依赖，改为人工或模型逐条自检。

## UI UX Pro Max（Next Level Builder）

- 来源：https://github.com/nextlevelbuilder/ui-ux-pro-max-skill
- 许可证：MIT（`LICENSES/ui-ux-pro-max-MIT.txt`）
- 使用方式：`assets/themes.css` 的颜色变量结构参考了其配色数据的字段划分；`references/checklist.md` 中部分交互、无障碍条目参考了其 UX 规范数据。
- 修改说明：未复制其配色数值和风格数据；全部 11 套主题的配色、字体、标志细节和立体主视觉为本 skill 原创。

## Lucide

- 来源：https://lucide.dev
- 许可证：ISC（`LICENSES/lucide-ISC.txt`）
- 使用方式：`assets/icons.svg` 收录了其中 70 个图标的原始路径，打包为 SVG symbol，未修改图形。
