# LandingEdu · AI学伴（GitHub Pages）

用于部署到 GitHub Pages 的静态站点包。你的站点地址：  
**https://simahe2025.github.io/landingAGI2025_AIlearning/**

## 快速发布（Branch 模式）
1. 在 GitHub 新建仓库：`simahe2025/landingAGI2025_AIlearning`。
2. 把本压缩包内的所有文件上传到仓库 `main` 分支根目录（或本地 `git push`）。
3. 打开 **Settings → Pages**：
   - Build and deployment: **Deploy from a branch**
   - Branch: `main`  ·  Folder: `/ (root)`
4. 稍等几分钟后访问：https://simahe2025.github.io/landingAGI2025_AIlearning/

> 如果页面提示 404，请在 Pages 设置里确认分支是否选择正确，或重新保存一次设置。

## 可选：GitHub Actions 自动部署
仓库包含 `.github/workflows/deploy.yml` 工作流（可选）。
- 默认在 push 到 `main` 时自动构建并发布到 Pages。
- 如果你选择 Branch 模式，可删除该目录或禁用工作流。

## 本包包含
- `index.html`（主页）
- `404.html`（未找到页面）
- `robots.txt`、`sitemap.xml`（SEO）
- `site.webmanifest`、`favicon.svg`
- `.nojekyll`
- `.github/workflows/deploy.yml`（可选）

---
Made with ❤️ for 师范教育。