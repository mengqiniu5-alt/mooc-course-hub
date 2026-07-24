 ---
 layout: default
 title: 优课资料站
 description: 优课联盟 (UOOC) 课程备考资料索引
 ---
 
 <!-- Header Section -->
 <div class="container-fluid">
   <div class="container">
     <div class="row" style="padding: 3rem 0; text-align: center;">
       <h1 style="font-size: 2.5rem; font-weight: 700; margin-bottom: 0.5rem;">优课资料站</h1>
       <p style="font-size: 1.2rem; color: #555; max-width: 600px; margin: 0 auto;">
         优课联盟 (UOOC) 课程备考资料索引 · 减少信息搜集成本
       </p>
     </div>
   </div>
 </div>
 
 <!-- About Section -->
 <div class="container-fluid" style="background: #f8f9fa; padding: 2rem 0;">
   <div class="container">
     <h2 style="font-size: 1.6rem; font-weight: 600;">关于本站</h2>
     <p>本站专注于 <strong>优课联盟 (UOOC)</strong> 平台的课程资料索引。</p>
     <p>优课联盟的许多课程采用开卷考试形式，学生需要提前下载课件、整理资料带入考场。本站的作用就是把这些课件集中起来——<strong>减少信息搜集成本，把时间留给复习本身。</strong></p>
     <p>所有资料由选课同学主动提供，整理后上传。如有新课程或更新资料，欢迎联系维护。</p>
   </div>
 </div>
 
 <!-- Skills Section -->
 <div class="container-fluid" style="padding: 2rem 0;">
   <div class="container">
     <h2 style="font-size: 1.6rem; font-weight: 600;">课程分类</h2>
     <div style="display: flex; flex-wrap: wrap; gap: 0.8rem; margin-top: 1rem;">
       {% for skill in site.data.skills %}
       <div style="background: #eef2f7; padding: 0.6rem 1.2rem; border-radius: 20px; font-size: 0.9rem;">
         <strong>{{ skill.name }}</strong>
         <span style="color: #888; font-size: 0.8rem; display: block; margin-top: 0.2rem;">{{ skill.description }}</span>
       </div>
       {% endfor %}
     </div>
   </div>
 </div>
 
 <!-- Courses Section -->
 <div class="container-fluid" style="background: #f8f9fa; padding: 2rem 0;">
   <div class="container">
     <h2 style="font-size: 1.6rem; font-weight: 600;">课程资料</h2>
     <p style="color: #666;">点击课程名即可下载资料；无资料的课程显示"待上传"。</p>
 
     {% for project in site.data.projects %}
     <div style="border-left: 4px solid #4a90d9; padding: 1rem 1.5rem; margin-bottom: 1rem; background: #fff; border-radius: 4px;">
       
       <div style="font-size: 1.15rem; font-weight: 700; margin-bottom: 0.3rem;">
         {% if project.materials and project.materials.size > 0 %}
           {% assign first_file = project.materials | first %}
           <a href="{{ site.baseurl }}/{{ first_file.path }}" download>
             ⬇ {{ project.name }}
           </a>
         {% else %}
           {{ project.name }}
           <span style="display: inline-block; margin-left: 0.5rem; padding: 0.05rem 0.5rem; background: #ffe0b0; color: #b55a00; border-radius: 10px; font-size: 0.75rem; font-weight: 600;">待上传</span>
         {% endif %}
       </div>
 
       <div style="font-size: 0.85rem; color: #888; display: flex; gap: 1rem; flex-wrap: wrap; margin-bottom: 0.3rem;">
         <span>{{ project.category }}</span>
         <span>更新: {{ project.updated }}</span>
         {% if project.status == "已更新" %}
           <span style="background: #e8f5e9; color: #2e7d32; padding: 0.1rem 0.5rem; border-radius: 10px;">已更新</span>
         {% else %}
           <span style="background: #fff3e0; color: #e65100; padding: 0.1rem 0.5rem; border-radius: 10px;">待更新</span>
         {% endif %}
       </div>
 
       <div style="font-size: 0.9rem; color: #444; margin: 0.3rem 0;">
         {{ project.description | newline_to_br }}
       </div>
 
       {% if project.materials and project.materials.size > 0 %}
       <div style="margin-top: 0.5rem; padding: 0.5rem 0.7rem; background: #f5f7fa; border-radius: 4px; font-size: 0.85rem;">
         <strong>资料文件：</strong>
         <ul style="margin: 0.3rem 0 0 0; padding-left: 1.2rem;">
         {% for file in project.materials %}
           <li style="margin: 0.2rem 0;">
             <a href="{{ site.baseurl }}/{{ file.path }}" download>
               📄 {{ file.name }}
               {% if file.size %}<span style="color: #999; font-size: 0.75rem;">({{ file.size }})</span>{% endif %}
             </a>
           </li>
         {% endfor %}
         </ul>
       </div>
       {% endif %}
 
     </div>
     {% endfor %}
   </div>
 </div>
 
 <!-- Contact Section -->
 <div class="container-fluid" style="padding: 2rem 0;">
   <div class="container" style="text-align: center;">
     <p>
       <a href="https://github.com/mengqiniu5-alt" style="color: #4a90d9; font-size: 1rem;">GitHub → mengqiniu5-alt</a>
     </p>
   </div>
 </div>
