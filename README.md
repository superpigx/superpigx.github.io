# 我的博客

基于 **Hugo + PaperMod 主题** 的 GitHub Pages 博客。

- Hugo 版本：`0.164.0`（最新）
- PaperMod 版本：`v8.0`（最新）
- 主题由 GitHub Actions 在云端自动拉取，无需本地 submodule。

## 目录结构

```
.
├── hugo.toml                 # 站点配置
├── content/
│   ├── posts/                # 文章放这里
│   │   └── hello-world.md
│   └── about.md              # 关于页
└── .github/workflows/
    └── deploy.yml            # 自动构建部署到 GitHub Pages
```

## 本地预览（可选，需先安装 Hugo 0.164.0+）

```bash
hugo server -D
```

## 发布流程

1. push 到 `master` 分支，GitHub Actions 自动构建并部署。
2. 在仓库 **Settings → Pages** 中，Source 选择 **GitHub Actions**。
3. 构建完成后访问 `https://superpigx.github.io`。

## 写新文章

把 Markdown 文件放到 `content/posts/`，`draft: false` 即发布。

## 配置修改

- 站点标题 / 描述：编辑 `hugo.toml` 的 `title`、`params.description`。
- 社交链接：编辑 `hugo.toml` 的 `[params.social]`。
- 菜单：编辑 `hugo.toml` 的 `[[menu.main]]`。
