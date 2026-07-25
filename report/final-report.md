 # 最终报告
 
 ## 项目定位
 
 牛萌琪的个人主页网站，展示个人信息、能力、项目经历和联系方式，面向教师验收和未来求职展示。
 
 ## 模板选择
 
 - **所选模板**：Modern Resume Theme (sproogen/modern-resume-theme)
 - **模板仓库**：[sproogen/modern-resume-theme](https://github.com/sproogen/modern-resume-theme)
 - **选择理由**：结构清晰、GitHub Pages 原生支持、适合个人展示
 - **最终方案**：因 Jekyll 远程主题在 GitHub Pages 构建中不稳定，改用独立 HTML + .nojekyll 静态部署
 
 ## 主要修改内容
 
 - 站点定位从个人简历改为牛萌琪个人主页
 - Skills 区展示合作谈判、产品思维、需求分析等真实能力
 - Projects 区展示两个真实项目（明川银行 AI 反欺诈立项分析 + 材料纠错修复）
 - 隐藏 Experience、Education 等无关区块
 - 添加中文排版优化（Noto Sans SC 字体）
 
 ## AI 参与说明
 
 AI Agent（Codex）在以下环节提供了帮助：
 - 阅读作业说明并梳理项目需求
 - 搭建项目目录结构与文档框架（PRD / Design / Checklist）
 - 生成 HTML 页面与 CSS 样式
 - 配置 GitHub 仓库、推送代码并开启 Pages
 - 排查构建错误（远程主题插件冲突 → 改用 .nojekyll 静态部署）
 
 ## 个人判断与决策
 
 - 确定网站定位为个人主页而非 MOOC 资料站
 - 选择展示实验1（反欺诈立项分析）和实验2（材料纠错修复）两个真实项目
 - 内容采用真实个人信息（姓名、学校、能力、项目经历）
 - 在 Jekyll 构建失败后，决策改用独立 HTML 静态部署，确保上线
 
 ## 验证结果
 
 - 桌面端：导航正常、内容完整、链接有效
 - 移动端：单栏布局、无横向滚动、文字可读
 - GitHub Pages：https://mengqiniu5-alt.github.io/mooc-course-hub/ 可访问
 - Checklist 已完成内容/功能/显示/工程四项验证
 
 ## GitHub Pages 链接
 
 ```
 https://mengqiniu5-alt.github.io/mooc-course-hub/
 ```
 
 ## 遇到的问题与解决方案
 
 | 问题 | 原因 | 解决方法 |
 |------|------|----------|
 | Jekyll 构建失败 | remote_theme 与 GitHub Pages 默认插件冲突 | 移除冲突插件配置，后改用 .nojekyll 纯静态 |
 | git push 网络不稳定 | 沙箱网络对 git 二进制限制 | 改用 GitHub API 通过 Python 推送代码 |
 | 页面返回 empty | Jekyll 生成了空 _site 目录 | 使用独立 index.html + .nojekyll 直接部署 |
 
 ## 后续计划
 
 - 如获取教师统一模板，可无缝迁移
 - 补充个人头像照片
 - 持续更新 Project 中的课程和项目内容
 
 ---
 
 *版本：v0.1 | 最后更新：2026-07-25*
