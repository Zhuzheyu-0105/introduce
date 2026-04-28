# 朱哲宇 — 个人作品集网站

> 纯静态 HTML/CSS 网站，无需构建，直接部署。

## 📁 目录结构

```
bushu/
├── index.html          ← 主页（作品集首页）
├── YAO/                ← YAO 儿童口腔训练器品牌页
│   └── index.html
├── Bi/                 ← Bi 鼻腔护理设备品牌页
│   └── index.html
├── olight/             ← O light 折叠灯品牌页（原"O light"，已去除空格）
│   └── index.html
├── images/             ← 首页图片资源
│   └── awards/
├── logo/               ← Logo 资源
└── 图片/               ← 公共图片
```

---

## 🚀 一键部署到 GitHub Pages

### 前提：安装 Git
下载地址：https://git-scm.com/download/win（安装时全部默认即可）

### 第一步：在 GitHub 创建仓库
1. 登录 https://github.com
2. 点右上角 **+** → **New repository**
3. 仓库名填：`你的用户名.github.io`（例：`zhuzheyu.github.io`）
4. 选择 **Public**
5. **不要**勾选"Add a README file"
6. 点 **Create repository**

### 第二步：在此目录打开 PowerShell，执行以下命令

```powershell
# 进入 bushu 目录
cd "D:\个人网站简历\bushu"

# 初始化 Git
git init
git add .
git commit -m "初始部署：朱哲宇个人作品集"

# 替换 YOUR_USERNAME 为你的 GitHub 用户名！
git remote add origin https://github.com/YOUR_USERNAME/YOUR_USERNAME.github.io.git
git branch -M main
git push -u origin main
```

### 第三步：开启 Pages
1. 进入 GitHub 仓库页面
2. 点 **Settings** → 左侧 **Pages**
3. Source 选 **Deploy from a branch**
4. Branch 选 **main**，Folder 选 **/ (root)**
5. 点 **Save**

等待约 1~3 分钟，网站上线地址：
```
https://YOUR_USERNAME.github.io
```

---

## 🔄 后续更新网站

修改文件后，在 `bushu/` 目录执行：

```powershell
git add .
git commit -m "更新内容描述"
git push
```

推送后 GitHub 自动重新部署，约 1 分钟生效。

---

## ✅ 部署前检查清单

- [x] `O light` 文件夹已重命名为 `olight`
- [x] `index.html` 中 `O light/index.html` 路径已修正为 `olight/index.html`
- [x] 所有图片均为相对路径（无本地盘符）
- [ ] 确认 GitHub 账号已注册
- [ ] 将 `YOUR_USERNAME` 替换为实际 GitHub 用户名

---

## 📋 页面访问路径

| 页面 | URL |
|------|-----|
| 主页 | `https://你.github.io/` |
| YAO 品牌页 | `https://你.github.io/YAO/` |
| Bi 品牌页 | `https://你.github.io/Bi/` |
| O light 品牌页 | `https://你.github.io/olight/` |
