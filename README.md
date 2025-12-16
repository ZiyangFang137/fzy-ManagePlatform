# 🎓 实训过程质量跟踪管理平台

> 企业培训三周后完成的前端管理系统大作业

## 📌 项目简介

**中北大学实训过程质量管理系统**，用于跟踪和管理学生的实训过程、技能评估和教学质量。

- ⏱️ **完成时间**：企业培训第 3 周
- 🎯 **核心目标**：学生管理、班级管理、教师管理、质量评估
- 💾 **技术特点**：全前端实现，无后端，数据前端模拟

---

## 🛠 技术栈

| 类型            | 技术                                    |
| --------------- | --------------------------------------- |
| **HTML/CSS/JS** | 页面基础三剑客                          |
| **框架**        | Layui v2.6.3 + jQuery 3.4.1             |
| **插件**        | wangEditor、ECharts、TreeTable、LayDate |
| **图标**        | Font Awesome 4.7.0                      |

---

## 📁 项目结构

```
ManagePlatform/
├── index.html              # 主页面（登录后的首页）
├── login.html              # 登录页面
│
├── api/                    # 模拟 API 数据 (JSON 格式)
│   ├── init.json          # 菜单初始化配置
│   ├── menus.json         # 菜单数据
│   ├── user.json          # 用户数据
│   ├── student.json       # 学生数据
│   └── ...                # 其他业务数据
│
├── page/                   # 核心业务页面
│   ├── home.html          # 仪表板（首页）
│   ├── form.html          # 表单示例
│   ├── table.html         # 表格示例
│   ├── upload.html        # 文件上传
│   └── ...
│
├── class/                  # 班级管理模块
│   ├── addclass.html      # 添加班级
│   └── changeclass.html   # 修改班级
│
├── student/               # 学生管理模块
│   ├── studentZC.html    # 学生注册
│   ├── studentCZ.html    # 学生查询
│   └── ...
│
├── teacher/               # 教师管理模块
│   ├── addteacher.html   # 添加教师
│   └── changeteacher.html # 修改教师
│
├── PQC/                   # 过程质量管控
│   ├── rTR.html          # 日常技术检查
│   ├── everyday.html     # 课前提问
│   ├── bExam.html        # 笔试
│   ├── mExam.html        # 面试
│   ├── daima.html        # 代码评审
│   └── simulate.html     # 模拟面试
│
├── zTeach/                # 教学质量管控
│   ├── zTeach.html       # 周教学计划
│   ├── zTeachZj.html     # 周教学总结
│   └── zTeachJL.html     # 教师打分记录
│
├── css/                   # 样式文件
│   ├── layuimini.css     # 主框架样式
│   ├── public.css        # 公共样式
│   └── themes/           # 主题配置
│
├── js/                    # 脚本文件
│   ├── lay-config.js     # Layui 配置
│   ├── statis/           # 统计相关脚本
│   └── lay-module/       # Layui 扩展模块
│
├── lib/                   # 第三方库
│   ├── layui-v2.6.3/    # Layui 框架（核心！）
│   ├── jquery-3.4.1/    # jQuery 库
│   ├── font-awesome-4.7.0/  # 图标库
│   └── jq-module/       # jQuery 插件
│
├── images/ & img/         # 图片资源
└── README.md             # 项目文档（你在看这个！）
```

---

## 🚀 快速开始

### 1️⃣ 本地运行

**方法一：用浏览器直接打开**

```bash
# 只需在浏览器中打开 login.html
# 推荐用 Chrome/Firefox/Edge（IE 会有兼容性问题）
```

**方法二：用本地 Web 服务器**（推荐）

```bash
# 用 Python 3
python -m http.server 8000

# 或用 Node.js 的 http-server
npx http-server

# 然后访问：http://localhost:8000
```

### 2️⃣ 登录系统

- **用户名**：任意（前端未做严格校验）
- **密码**：任意
- 点击 **登录** 进入首页

### 3️⃣ 使用功能

- 左侧菜单：点击菜单项切换不同页面
- 表格操作：新增、编辑、删除、搜索功能
- 表单提交：填写表单后点击提交（数据仅存储在浏览器缓存）
- 主题切换：右上角"配色方案"可切换界面颜色

---

## 📚 核心功能模块

### 1. **学生管理** 👥

- ✅ 学生账号注册
- ✅ 学生信息查询
- ✅ 学生详情修改
- ✅ 学生删除

### 2. **班级管理** 📚

- ✅ 班级信息添加
- ✅ 班级信息修改
- ✅ 班级信息查询

### 3. **教师管理** 👨‍🏫

- ✅ 教师账号录入
- ✅ 教师信息修改
- ✅ 教师信息查询

### 4. **过程质量管控** ✅

- ✅ 日常技术检查记录
- ✅ 每日课前提问
- ✅ 阶段笔试管理
- ✅ 阶段面试管理
- ✅ 代码评审
- ✅ 模拟面试

### 5. **教学质量管控** 📊

- ✅ 周教学计划制定
- ✅ 周教学总结记录
- ✅ 教师打分记录查询

### 6. **数据统计** 📈

- ✅ 可视化图表展示（ECharts）
- ✅ 表格数据导出
- ✅ 性能数据分析

---

## 💡 关键学习要点

### 第 1 周：HTML/CSS 基础

- ✏️ 编写语义化 HTML 结构
- 🎨 使用 CSS 实现布局与样式
- 📱 理解响应式设计（media query）

### 第 2-3 周：JavaScript + Layui 框架

- 🔧 DOM 操作与事件监听
- 📤 表单验证与提交
- 🎯 使用 Layui 组件（表格、表单、弹窗等）
- 💾 浏览器本地存储（localStorage/sessionStorage）
- 🔄 模拟 API 数据交互（AJAX 基础）

### 项目中用到的 JS 技能

```javascript
// 1. 事件监听与委托
$(".layui-table-tool").on("click", ".layui-btn", function () {
  // 处理按钮点击
});

// 2. 表单验证
layui.form.on("submit(filter)", function (data) {
  // 验证表单数据
});

// 3. 本地存储
sessionStorage.setItem("key", value);
var data = JSON.parse(localStorage.getItem("key"));

// 4. 动态 HTML 拼接
var html =
  "<table>" +
  dataList.map((item) => "<tr><td>" + item.name + "</td></tr>").join("") +
  "</table>";

// 5. 条件判断与循环
dataList.forEach(function (item, index) {
  if (item.status == "active") {
    // 处理逻辑
  }
});
```

---

## 🤔 遇到的难点 & 解决方案

### 难点 1：Layui 框架学习曲线陡

**问题**：Layui 有众多组件（表格、表单、弹窗等），各有不同用法，初学者容易混乱。

**解决方案**：

- 📖 阅读 Layui 官方文档示例
- 🎬 跟着教程视频逐个学习组件
- 💻 在 `page/` 目录下创建独立示例页面进行测试
- ✏️ 记录常用代码片段备用

### 难点 2：页面间数据传递困难

**问题**：从学生列表页跳到详情页，如何携带学生 ID？

**解决方案**：

- ✅ 使用 `sessionStorage` 存储临时数据
- ✅ URL 查询参数传递（`?id=123`）
- ✅ 利用 Layui 的 `layer.open()` 嵌入 iframe

```javascript
// 示例：通过 URL 传递 ID
function goDetail(id) {
  // 方案 1：URL 参数
  window.location.href = "detail.html?id=" + id;

  // 方案 2：sessionStorage
  sessionStorage.setItem("currentStudentId", id);
  layer.open({
    type: 2,
    content: "detail.html",
  });
}
```

### 难点 3：多个表格和表单管理混乱

**问题**：项目中有 10+ 个表格和表单，代码重复多，维护困难。

**解决方案**：

- 📋 提取通用函数（`loadTable()`, `submitForm()` 等）
- 🏷️ 使用统一的数据结构规范
- 📝 在 `js/lay-config.js` 中配置全局变量和方法

### 难点 4：调试时数据丢失

**问题**：刷新页面后，本地 JS 变量全部丢失，无法恢复状态。

**解决方案**：

- 💾 使用 `localStorage` 持久化重要数据
- 🔄 页面加载时从 localStorage 恢复状态
- 🛠️ 浏览器开发者工具（F12）查看本地存储

```javascript
// 初始化时恢复数据
window.onload = function () {
  var savedData = localStorage.getItem("userList");
  if (savedData) {
    userList = JSON.parse(savedData);
  }
};

// 修改数据时保存
function updateStudent(id, name) {
  var student = findStudent(id);
  student.name = name;
  localStorage.setItem("userList", JSON.stringify(userList));
}
```

### 难点 5：样式兼容性问题

**问题**：在 Chrome 中正常，IE 中显示错乱。

**解决方案**：

- ✅ 优先使用 Layui 提供的样式类，避免自定义 CSS
- ✅ 测试常见浏览器（Chrome、Firefox、Safari）
- ✅ 使用 CSS 前缀处理过时特性：`-webkit-`, `-moz-` 等

---

## 🐛 常见问题 (FAQ)

### Q1: 页面打开是空白的，怎么办？

**A**:

1. 检查浏览器控制台（F12 → Console）有没有红色错误
2. 确保所有资源文件路径正确（特别是 lib/ 目录）
3. 用 Web 服务器运行而不是直接打开 HTML 文件

### Q2: 表格没有数据，只有表头？

**A**:

1. 检查 `api/` 中对应的 JSON 数据文件是否存在
2. 检查 AJAX 请求路径是否正确
3. 在浏览器中直接访问 JSON 文件 URL 看是否能加载

### Q3: 如何添加新的菜单项？

**A**: 编辑 `api/init.json`，在 `menuInfo` 数组中添加新对象：

```json
{
  "title": "我的功能",
  "href": "mypage/mypage.html",
  "icon": "fa fa-star",
  "target": "_self"
}
```

### Q4: 如何修改系统主题颜色？

**A**:

- 方法 1：右上角"配色方案"按钮手动切换
- 方法 2：编辑 `css/themes/default.css` 修改全局色值

### Q5: 数据会保存吗？

**A**:

- ❌ **不会**。所有数据都是前端内存存储，刷新页面就丢失了
- 💡 可以用 `localStorage` 实现简单持久化，但仍需后端数据库才能真正保存

---

## 📖 学习资源

### 推荐教程

- **Layui 官方文档**：http://www.layui.com/doc/
- **MDN JavaScript 教程**：https://developer.mozilla.org/zh-CN/docs/Web/JavaScript
- **jQuery 中文文档**：https://jquery.cuishifeng.cn/

### 代码参考

- `page/form.html` - 表单组件用法示例
- `page/table.html` - 表格组件用法示例
- `page/layer.html` - 弹窗组件用法示例
- `PQC/` 目录 - 真实业务页面示例

---

## ✨ 项目亮点

✅ **全前端实现** - 无需后端，快速验证想法  
✅ **高仿真管理系统** - 涵盖 6 大业务模块，接近真实项目  
✅ **代码结构清晰** - 按功能模块分目录，易于维护  
✅ **友好的 UI 设计** - 采用 Layui 企业级组件，美观专业  
✅ **实用的学习案例** - 集成 HTML/CSS/JS 三大要点，是入门好教材

---

## 🎯 后续改进方向

如果继续深化这个项目，可以考虑：

| 方向         | 实现难度 | 描述                                  |
| ------------ | -------- | ------------------------------------- |
| 后端接口集成 | ⭐⭐⭐   | 使用 Node.js/Java/Python 实现真实 API |
| 用户认证     | ⭐⭐     | 添加登录验证，生成 token 认证         |
| 数据持久化   | ⭐⭐⭐   | 接入 MySQL/MongoDB 数据库             |
| 权限管理     | ⭐⭐⭐   | 根据角色限制功能访问权限              |
| 移动端适配   | ⭐⭐     | 优化响应式设计，完善手机体验          |
| 单元测试     | ⭐⭐⭐   | 使用 Jest/Mocha 框架编写测试用例      |
| 前端工程化   | ⭐⭐⭐⭐ | 引入 Webpack、Babel、ESLint 等工具    |

---

## 👩‍💼 关于作者

- **学生**：软件工程大二女生
- **培训**：企业上门培训 3 周
- **学习成果**：从零基础到独立完成一个完整的管理系统前端项目
- **技能获得**：HTML/CSS/JavaScript/Layui 框架/前端工程化思维

> _"三周的培训，让我从对前端一无所知，到能独立完成一个真实项目。最大的收获不仅是技术本身，更是学会了如何系统地学习和解决问题。"_

---

## 📄 许可证

本项目仅供学习和参考使用。  
如用于商业用途，请确保遵守 Layui、jQuery 等第三方库的许可证要求。

---

## 📞 更新日志

| 版本 | 日期       | 内容                         |
| ---- | ---------- | ---------------------------- |
| v1.0 | 2025-12-16 | 项目初始化，完成核心功能开发 |
| v1.1 | 待定       | 计划添加数据导出功能         |
| v2.0 | 待定       | 计划后端接口对接             |

---

<div align="center">

**感谢企业老师的耐心指导和同学们的鼓励支持！** 🙏

⭐️ 如果这个项目对你有帮助，请给个 Star 吧！

</div>
