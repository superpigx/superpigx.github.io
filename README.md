# 我的博客

基于 **Hugo + Stack 主题** 的 GitHub Pages 博客。

## 目录结构

```
.
├── hugo.toml                 # 站点配置
├── content/
│   ├── posts/                # 文章放这里
│   │   └── hello-world.md
│   └── about.md              # 关于页
├── themes/
│   └── hugo-theme-stack      # 主题（git submodule）
└── .github/workflows/
    └── deploy.yml            # 自动构建部署到 GitHub Pages
```

## 本地预览（可选，需先安装 Hugo）

```bash
hugo server -D
```

## 发布流程

1. 在 GitHub 新建仓库（仓库名 `username.github.io` 或用任意名并开启 Pages）。
2. 提交并 push 到 `main` 分支（主题由 GitHub Actions 在云端自动拉取，无需本地处理 submodule）。
4. 在仓库 Settings → Pages 中，Source 选择 "GitHub Actions"。

## 写新文章

把 Markdown 文件放到 `content/posts/`，`draft: false` 即发布。

## 配置修改

- 站点标题 / 描述：编辑 `hugo.toml` 顶部的 `title`、`params.description`。
- 社交链接 / 评论：在 `hugo.toml` 中按注释填写。
- 记得把配置里的 `username` 替换成你的 GitHub 用户名。
