 # 牛萌琪 · 个人主页
 
 > OPC-AI 培训营 · 模块三实验课作业
 > 用规范化 AI 开发流程完成个人网站
 
 ## 项目说明
 
 牛萌琪的个人简历/作品集网站。展示个人信息、能力、项目经历和联系方式。
 
 ## 所用模板
 
 - **模板仓库**：[sproogen/modern-resume-theme](https://github.com/sproogen/modern-resume-theme)
 - **选择理由**：结构清晰、GitHub Pages 原生支持、适合做个人展示型站点
 
 ## 主要修改内容
 
 - 站点定位从 MOOC 课程资料站改为个人主页
 - 替换所有个人信息（姓名、简介、技能、项目）
 - Skills 区展示合作谈判、产品思维、需求分析等真实能力
 - Projects 区展示明川银行 AI 反欺诈预警系统（实验1+实验2）和个人网站项目
 - 隐藏 Experience、Education 等无关区块
 
 ## GitHub Pages 正式链接
 
 **[https://mengqiniu5-alt.github.io/mooc-course-hub/](https://mengqiniu5-alt.github.io/mooc-course-hub/)**
 
 ## 隐私说明
 
 本仓库不包含密码、API Key、Token、.env 文件、课程邀请码、个人敏感信息。
 
 ## 项目结构
 
 ```
 个人网站项目/
 ├─ _config.yml          # Jekyll 配置
 ├─ index.md             # 首页
 ├─ _data/
 │  ├─ skills.yml        # 个人能力
 │  └─ projects.yml      # 项目经历
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
