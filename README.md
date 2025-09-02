# LandingEdu · AI学伴

面向师范大学教师与学生的 **AI 教学与生活应用** 站点。已包含：
- 首页（Tailwind CDN，无需构建）
- SVG 横幅、柔光网格背景、暗色模式
- 模块：AI 工具箱 / 教学应用案例 / 学习资源 / 我的项目展示 / 社区交流（占位）
- GitHub Pages 所需的**配套文件**：`404.html`、`robots.txt`、`sitemap.xml`、`site.webmanifest`、`favicon.svg`、`.nojekyll`、可选的 GitHub Actions 工作流。

> 你可以直接把本仓库作为 GitHub Pages 发布；或将这里的文件复制到你已有的仓库。

---

## 目录结构

```
.
├─ index.html                 # 主页（可直接替换为你在画布中的最新版 index.html）
├─ 404.html                   # 404 友好页（返回首页）
├─ robots.txt                 # 爬虫策略（已开放全站）
├─ sitemap.xml                # 站点地图（请替换成你的用户名/仓库名）
├─ site.webmanifest           # PWA/图标配置
├─ favicon.svg                # 站点图标（LE 徽标，可自行替换）
├─ .nojekyll                  # 关闭 Jekyll 处理，确保下划线/构建产物可访问
└─ .github/
   └─ workflows/
      └─ deploy.yml          # 可选：自动部署到 GitHub Pages 的工作流
```

> 注意：`index.html` 已内置 Tailwind CDN 与示例占位横幅。**建议把你在 ChatGPT 画布中的最新版 `index.html` 覆盖到这里**，即可得到完全一致的页面。

---

## 本地预览

直接用浏览器打开 `index.html` 即可。  
或者 VS Code + Live Server：右下角 **Go Live**。

---

## 发布到 GitHub Pages

### 方案 A（最简单）：Settings 启用

1. 推送到 GitHub：

   ```bash
   git init
   git add .
   git commit -m "init: LandingEdu on GitHub Pages"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-repo>.git
   git push -u origin main
   ```

2. 打开仓库 **Settings → Pages**：
   - **Source** 选择 *Deploy from a branch*
   - Branch 选择 **main / / (root)**
   - 保存后，等待几分钟，访问：  
     `https://<your-username>.github.io/<your-repo>/`

### 方案 B（自动）：GitHub Actions

- 已包含 `.github/workflows/deploy.yml`，默认在 `main` 分支有推送时自动部署。  
- 进入 **Settings → Pages**，将 **Build and deployment → Source** 设为 **GitHub Actions**。

> 两种方案二选一即可。

---

## 自定义与替换

- **SVG 横幅**：在 `index.html` 中搜索注释“SVG banner”，将其替换为你画布中的完整 SVG 片段。
- **站点标题/描述**：编辑 `<title>` 与 `<meta name="description">`。
- **自定义域名**：在仓库根目录添加 `CNAME` 文件（仅一行写你的域名），并将域名解析到 `username.github.io`。
- **Sitemap**：将 `sitemap.xml` 与 `robots.txt` 中的 `<your-username>/<your-repo>` 替换为真实值。
- **图标**：把 `favicon.svg` 换成你的徽标；必要时在 `site.webmanifest` 更新颜色。

---

## 版权与合规

- 页面示例图片来自 **Pixabay**，遵循其免费许可（可商用、无需署名）。  
- 你若搬运视频/博客，请**注明来源并尊重版权**。
- 本模板默认使用 **MIT License**（可按需替换）。

---

## License

MIT © 2025 <你的名字>
