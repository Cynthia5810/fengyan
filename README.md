# 个人网站（静态版）

这是一个可直接部署到 GitHub Pages 的单页网站（`index.html` + `styles.css` + `script.js`）。

## 本地预览
直接双击 `index.html` 打开，或使用任意静态服务器：
```bash
python -m http.server 8080
```

## 部署到 GitHub Pages
1. 新建仓库：建议命名 `yourname.github.io`（用户站点）。
2. 把本目录所有文件推送到仓库根目录（分支 `main`）。
3. 仓库 **Settings → Pages**：Source 选 `Deploy from a branch`，Branch 选 `main`，Folder 选 `/ (root)`。
4. 1–3 分钟后访问 `https://yourname.github.io`。

> 若你是“项目站点”（仓库名不是 `yourname.github.io`），访问链接为 `https://yourname.github.io/<repo-name>/`。

## 国内加速（可选）
可在 Gitee 上建立镜像仓库并启用 Gitee Pages；或使用我提供的“GitHub→Gitee 自动同步工作流”同步国内站点。

## 自定义
- 修改文案：编辑 `index.html` 中的内容即可。
- 主题配色：在 `styles.css` 的 `:root` 里调整色值。
- 简历下载：将仓库中加入 `resume.pdf`，按钮会自动指向该文件。

## 常见问题（404 排查）
- `index.html` 必须在仓库根目录。
- Pages 的 Source/Branch/Folder 要和实际位置一致。
- 根目录可添加空文件 `.nojekyll` 以避免 Jekyll 忽略下划线资源。
