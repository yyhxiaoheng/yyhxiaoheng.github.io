# 黑b李果 - 个人博客

一个纯静态的个人博客页面，使用原生 HTML + CSS + JavaScript 构建，无任何依赖，可直接部署到 GitHub Pages。

## 文件结构

```
blog-static/
├── index.html      # 主页面
├── style.css       # 样式文件
├── script.js       # 交互脚本
└── README.md       # 说明文档
```

## 功能特性

- 🎨 现代化渐变设计风格
- 📱 完整响应式布局（支持移动端）
- ✨ 滚动入场动画效果
- 🧭 导航栏滚动高亮
- 📍 平滑滚动锚点跳转
- 🔝 回到顶部按钮
- 🍔 移动端汉堡菜单
- 🖼️ 三张个人照片展示（头像 + 背景 + 生活照）

## 本地预览

直接用浏览器打开 `index.html` 即可预览。

或使用本地服务器：

```bash
# Python
python3 -m http.server 8080

# Node.js
npx serve .
```

然后访问 http://localhost:8080

## 部署到 GitHub Pages

### 方法一：手动上传

1. 在 GitHub 创建新仓库（例如 `my-blog`）
2. 将本目录所有文件上传到仓库
3. 进入仓库 Settings → Pages
4. Source 选择 `Deploy from a branch`
5. Branch 选 `main` / `root`，点击 Save
6. 等待 1-2 分钟，访问 `https://你的用户名.github.io/仓库名/`

### 方法二：Git 命令行

```bash
# 进入项目目录
cd blog-static

# 初始化 Git
git init
git add .
git commit -m "init personal blog"
git branch -M main

# 关联远程仓库（替换为你的仓库地址）
git remote add origin https://github.com/你的用户名/仓库名.git
git push -u origin main
```

然后在仓库设置中开启 GitHub Pages 即可。

## 自定义修改

- 修改文字内容：编辑 `index.html`
- 修改颜色样式：编辑 `style.css` 顶部 `:root` 中的 CSS 变量
- 修改图片：替换 `index.html` 中的图片 URL
