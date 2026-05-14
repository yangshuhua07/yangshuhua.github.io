---
layout: default
title: 首页 | Your Name
---

<section id="about" class="flex flex-col md:flex-row items-center gap-8 py-4">
  <div class="w-32 h-32 rounded-full bg-gradient-to-tr from-blue-600 to-indigo-600 flex-shrink-0 flex items-center justify-center text-white text-3xl font-bold shadow-lg">
    YN
  </div>
  <div class="space-y-3">
    <h1 class="text-3xl font-extrabold text-gray-900 tracking-tight">Your Name</h1>
    <p class="text-sm text-gray-500 font-medium">学术研究员 / 软件开发工程师</p>
    <p class="text-gray-600 leading-relaxed text-sm">
      目前专注于<b>区域经济学</b>与<b>数字创新网络</b>的计量分析研究。同时具备全栈后端开发与底层调试能力，擅长将定量分析方法（如 ERGM、网络拓扑）与高性能数据处理技术相结合，探索数字经济时代的区域协同演化。
    </p>
    <div class="flex gap-4 text-gray-500 text-sm pt-1">
      <a href="mailto:your.email@example.com" class="hover:text-blue-600"><i class="fa-solid fa-envelope"></i> 邮箱</a>
      <a href="https://github.com" class="hover:text-black"><i class="fa-brands fa-github"></i> GitHub</a>
    </div>
  </div>
</section>

---

### <i class="fa-solid fa-book-bookmark text-blue-600 mr-2"></i> 研究成果 (Publications)
<div class="space-y-4 mt-4">
{% for pub in site.data.publications %}
  <div class="border-l-2 border-blue-500 pl-4 py-1">
    <h4 class="font-semibold text-gray-900 text-base">{{ pub.title }}</h4>
    <p class="text-xs text-gray-600 mt-1">{{ pub.authors }}</p>
    <p class="text-xs text-gray-400 mt-0.5"><i>{{ pub.journal }}</i>, {{ pub.year }} · <span class="text-blue-600 font-medium">{{ pub.status }}</span></p>
  </div>
{% endfor %}
</div>

---

### <i class="fa-solid fa-laptop-code text-indigo-600 mr-2"></i> 技术与开源项目 (Projects)
<div class="grid md:grid-cols-2 gap-4 mt-4">
{% for proj in site.data.projects %}
  <div class="p-4 bg-white border border-gray-100 rounded-lg shadow-xs">
    <span class="text-[10px] font-bold text-indigo-600 bg-indigo-50 px-2 py-0.5 rounded">{{ proj.tech }}</span>
    <h4 class="font-bold text-gray-900 mt-2 text-sm">{{ proj.name }}</h4>
    <p class="text-xs text-gray-600 mt-1 leading-relaxed">{{ proj.desc }}</p>
  </div>
{% endfor %}
</div>

---

### <i class="fa-solid fa-bars-progress text-emerald-600 mr-2"></i> 技术栈 (Skills)
* **研究方法**: 计量经济学 / 指数随机图模型 (ERGM) / 空间网络分析 / 文本挖掘与文本分析
* **后端开发**: Node.js / Python / 数据库系统架构 (SQLite / MySQL) / 复杂业务逻辑设计
* **底层与调试**: 系统调试 (LLDB) / 数据逆向分析 / 二进制原始传感器数据流处理
