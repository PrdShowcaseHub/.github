# 📁 .github

> PrdShowcaseHub 组织的 GitHub 配置中心

## 📖 关于此仓库

此仓库包含 PrdShowcaseHub 组织的 GitHub 社区健康文件和元数据配置，主要包括：

- **组织首页内容**：位于 [`profile/README.md`](profile/README.md)，展示在组织首页 `https://github.com/PrdShowcaseHub`
- **组织级 GitHub Actions 工作流模板**：位于 [`.github/workflows/`](.github/workflows/)
- **其他组织级配置文件**

## 📂 目录结构
```
.github/
├── profile/
│ └── README.md # 组织首页展示内容
├── workflows/
│ └── update-repo-list.yml # 自动更新项目导航列表
└── README.md # 本文件
```

## 🚀 工作流说明

### update-repo-list.yml

定时扫描组织下的所有公开仓库，自动更新 `profile/README.md` 中的项目导航列表。

- **触发方式**：每日 UTC 0:00 自动运行，或手动触发
- **使用的 Action**：[koj-co/readme-repos-list](https://github.com/marketplace/actions/readme-repos-list)
- **更新内容**：拉取组织下所有公开仓库，生成带链接的卡片列表

## 🤝 贡献指南

如需修改组织首页内容，请编辑 `profile/README.md` 文件并提交 PR。

> ⚠️ **注意**：`profile/README.md` 中 `<!-- start: readme-repos-list -->` 和 `<!-- end: readme-repos-list -->` 标记之间的内容由 GitHub Actions 自动生成，请勿手动编辑。
