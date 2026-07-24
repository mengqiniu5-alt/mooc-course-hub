 # 设计说明 (Design Document)
 
 ## 1. 页面区块与浏览顺序
 
 单页式设计，从上到下排列：
 
 1. **Hero** — 姓名、学校专业、一句话定位
 2. **About** — 个人简介
 3. **Skills** — 真实能力列表
 4. **Projects** — 项目经历卡片
 5. **Contact** — GitHub 链接
 
 ## 2. 颜色、字体与整体风格
 
 | 维度 | 方案 |
 |------|------|
 | 风格 | 简洁专业，偏商务/学术 |
 | 字体 | 系统无衬线 + Noto Sans SC / PingFang SC 中文优化 |
 
 ## 3. 响应式要求
 
 - 桌面端（≥1024px）：多栏布局，内容居中
 - 移动端（<768px）：单栏堆叠，无横向滚动
 
 ## 4. 关键文件
 
 | 文件 | 职责 |
 |------|------|
 | `_config.yml` | Jekyll 配置 |
 | `index.md` | 首页内容 |
 | `_data/skills.yml` | 个人能力数据 |
 | `_data/projects.yml` | 项目经历数据 |
 | `assets/css/main.scss` | 中文排版优化 |
 | `docs/` | PRD/Design/Checklist |
 | `report/final-report.md` | 最终报告 |
 | `screenshots/` | 截图证据 |
 
 ## 5. 保留与修改
 
 **保留**：布局框架、导航、响应式策略、Pages 配置
 **修改**：站点名称、Hero 内容、Skills（个人能力）、Projects（真实项目）
 
 ## 6. 素材来源
 
 - 图标：Font Awesome（模板内置）
 - 头像：待添加
 - 字体：Google Fonts 开源字体
 
 *版本：v0.3 | 最后更新：2026-07-24*
