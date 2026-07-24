 # 设计说明 (Design Document)
 
 ## 1. 页面区块与浏览顺序
 
 单页式设计，从上到下：
 
 1. **Hero** — "优课资料站"，一句话定位
 2. **About** — 站点定位、使命（减少信息搜集成本）
 3. **Skills** — 课程分类
 4. **Projects** — 课程资料卡片（含文件列表）
 5. **Contact** — GitHub 链接
 
 ---
 
 ## 2. 视觉风格
 
 | 维度 | 方案 |
 |------|------|
 | 风格 | 简洁、信息导向 |
 | 主色调 | Modern Resume Theme 默认蓝色 (#4a90d9) |
 | 字体 | 系统默认 + Noto Sans SC / PingFang SC |
 
 ---
 
 ## 3. 响应式
 
 - 桌面 (≥1024px)：网格分类 + 卡片列表
 - 移动 (<768px)：单栏堆叠，导航折叠
 
 ---
 
 ## 4. 关键文件
 
 | 文件 | 职责 |
 |------|------|
 | `_config.yml` | Jekyll 配置 |
 | `index.md` | 首页 |
 | `_data/skills.yml` | 课程分类数据 |
 | `_data/projects.yml` | 课程资料数据 |
 | `assets/css/main.scss` | 自定义样式 |
 | `assets/course-materials/` | 课件文件存储 |
 
 ---
 
 ## 5. 资料存储方案
 
 ```
 assets/course-materials/课程名/资料文件.pdf
 ```
 
 资料由用户提供 → 我上传到对应目录 → 更新 projects.yml 中的 materials 字段 → 提交推送。
 主题已配置为排除 docs/、report/、screenshots/ 目录，资料目录在构建范围内，可通过 Pages 直接访问。
 
 ---
 
 *版本：v1.0 | 最后更新：2026-07-24*
 *主要变更：聚焦优课联盟、增加资料存储方案、移除多平台聚合定位*
