 # 优课资料站
 
 > OPC-AI 培训营 · 模块三实验课作业
 > 用规范化 AI 开发流程完成个人网站
 
 ## 项目说明
 
 专注于 **优课联盟 (UOOC)** 平台的课程备考资料索引。
 开卷考试前一站式获取课件，减少信息搜集成本。
 
 ## 所用模板
 
 - **模板仓库**：[sproogen/modern-resume-theme](https://github.com/sproogen/modern-resume-theme)
 - **模板类型**：Jekyll 主题（remote_theme）
 - **选择理由**：结构清晰、GitHub Pages 原生支持、适合做信息展示型站点
 
 ## 主要修改内容
 
 - 站点定位从个人简历改为优课联盟资料索引
 - Skills 区改为课程分类
 - Projects 区改为课程资料条目卡片（含文件列表、下载链接）
 - 隐藏 Experience、Education 等无关区块
 - 添加自定义 CSS 优化中文排版和资料卡片样式
 - 支持 materials 字段展示可下载文件
 
 ## GitHub Pages 正式链接
 
 **[https://mengqiniu5-alt.github.io/mooc-course-hub/](https://mengqiniu5-alt.github.io/mooc-course-hub/)**
 
 ## 资料目录结构
 
 ```
 assets/course-materials/
 ├── 军事理论/
 │   └── 军事理论.pdf
 ├── 大学生心理健康/
 │   └── ...（待上传）
 ├── 中国传统文化/
 ├── 创新创业基础/
 └── 高等数学（上）/
 ```
 
 ## 本地预览
 
 需要 Ruby + Jekyll 环境：
 
 ```bash
 bundle install
 bundle exec jekyll serve
 ```
 
 ## 隐私说明
 
 本仓库不包含密码、API Key、Token、.env 文件、课程邀请码、个人敏感信息。
 
 ## 项目结构
 
 ```
 优课资料站/
 ├─ _config.yml
 ├─ index.md
 ├─ _data/
 │  ├─ skills.yml
 │  └─ projects.yml
 ├─ assets/
 │  ├─ css/main.scss
 │  ├─ images/
 │  └─ course-materials/
 ├─ Gemfile
 ├─ README.md
 ├─ docs/
 └─ report/
 ```
 
 ## 许可证
 
 MIT License · 基于 sproogen/modern-resume-theme 修改
