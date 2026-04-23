# RPA 应用场景库 - 发布指南

## 方式一：GitHub Pages（推荐，免费）

### 步骤 1：创建 GitHub 仓库

1. 打开 https://github.com/new
2. Repository name 填写：`rpa-scenarios`
3. 选择 Public
4. 点击 Create repository

### 步骤 2：上传文件

**方法 A：网页直接上传（最简单）**
1. 进入刚创建的仓库
2. 点击 "Add file" → "Upload files"
3. 将 `C:\Users\10540\.qclaw\workspace\rpa-scenarios-page\index.html` 拖入
4. 点击 "Commit changes"

**方法 B：命令行上传**
```bash
cd C:\Users\10540\.qclaw\workspace\rpa-scenarios-page
git init
git add .
git commit -m "Add RPA scenarios page"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/rpa-scenarios.git
git push -u origin main
```

### 步骤 3：开启 GitHub Pages

1. 进入仓库 Settings
2. 左侧菜单找到 "Pages"
3. Source 选择 "Deploy from a branch"
4. Branch 选择 "main"，文件夹选择 "/ (root)"
5. 点击 Save

### 步骤 4：获取访问链接

几分钟后，访问地址为：
```
https://YOUR_USERNAME.github.io/rpa-scenarios/
```

---

## 方式二：Netlify（更快）

### 步骤 1：注册 Netlify
1. 打开 https://app.netlify.com/signup
2. 用 GitHub 账号登录

### 步骤 2：拖拽部署
1. 登录后，点击 "Add new site" → "Deploy manually"
2. 将 `C:\Users\10540\.qclaw\workspace\rpa-scenarios-page` 文件夹拖入
3. 等待部署完成
4. 获得类似 `https://random-name.netlify.app` 的访问链接

---

## 方式三：Vercel（国内访问快）

### 步骤 1：注册 Vercel
1. 打开 https://vercel.com/signup
2. 用 GitHub 账号登录

### 步骤 2：导入项目
1. 点击 "Add New" → "Project"
2. 选择 GitHub 仓库
3. 点击 Deploy

---

## 文件位置

已准备好的文件：
```
C:\Users\10540\.qclaw\workspace\rpa-scenarios-page\index.html
```

---

## 建议

- **推荐 GitHub Pages**：免费、稳定、链接规范
- **推荐 Netlify**：部署最快，适合快速分享
- **推荐 Vercel**：国内访问速度快

---

## 访问效果

发布后，任何人通过链接即可访问：
- 左侧可筛选板块和适配模式
- 支持搜索
- 支持导出 CSV
- 点击查看详情
