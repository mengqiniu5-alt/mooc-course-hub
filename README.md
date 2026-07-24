 # MOOC 课程资料站
 
 > OPC-AI 培训营 · 模块三实验课作业
 > 用规范化 AI 开发流程完成个人网站
 
 ## 项目说明
 
 聚合主流 MOOC 平台（中国大学 MOOC、Coursera、edX 等）最新课程资料，面向大学生提供按领域分类的课程索引。
 
 ## 所用模板
 
 - **模板仓库**：[sproogen/modern-resume-theme](https://github.com/sproogen/modern-resume-theme)
 - **模板类型**：Jekyll 主题（remote_theme）
 - **选择理由**：结构清晰、GitHub Pages 原生支持、适合做信息展示型站点
 
 ## 主要修改内容
 
 - 站点定位从个人简历改为 MOOC 课程资料聚合
 - Skills 区改为课程分类（8 个领域）
 - Projects 区改为课程资料条目卡片
 - 隐藏 Experience、Education、Certifications 等无关区块
 - 添加自定义 CSS 优化中文排版和课程卡片样式
 - 规范中文混排字体栈
 
 ## GitHub Pages 正式链接
 
 > 部署后填写：`https://[你的用户名].github.io/[仓库名]/`
 
 ## 本地预览
 
 需要 Ruby + Jekyll 环境：
 
 ```bash
 bundle install
 bundle exec jekyll serve
 ```
 
 浏览器打开 http://127.0.0.1:4000
 
 ## 隐私说明
 
 本仓库不包含密码、API Key、Token、.env 文件、课程邀请码、个人敏感信息。
 
 ## 项目结构
 
 ```
 个人网站项目/
 ├─ _config.yml          # Jekyll 配置
 ├─ index.md             # 首页
 ├─ _data/
 │  ├─ skills.yml        # 课程分类
 │  └─ projects.yml      # 课程资料列表
 ├─ assets/
 │  ├─ css/main.scss     # 自定义样式
 │  └─ images/           # 图片资源
 ├─ Gemfile              # 构建依赖
 ├─ README.md
 ├─ docs/
 │  ├─ prd.md
 │  ├─ design.md
 │  └─ checklist.md
 ├─ report/
 │  └─ final-report.md
 └─ screenshots/
 ```
 
 ## 许可证
 
 MIT License · 基于 sproogen/modern-resume-theme 修改
