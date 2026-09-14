# 我的游戏分享站

一个用于分享个人浏览器小游戏和 AI 叙事实验的静态站点。打开首页即可试玩，无需安装 Node.js、数据库或其他运行时。

## 在线入口

部署后访问：`https://<你的用户名>.github.io/<仓库名>/`

首页：[`index.html`](./index.html)

## 作品

| 作品 | 介绍 | 入口 |
| --- | --- | --- |
| 江湖风云模拟 | 古风开放世界文字 RPG，支持 NPC 关系、记忆、背包、存档和 AI 对话 | [`GD3.9.html`](./GD3.9.html) |
| 现代人生模拟 | 以工作、关系和城市生活为主题的互动人生故事 | [`shv-modern4.1.html`](./shv-modern4.1.html) |
| 修仙问道模拟 | 围绕功法、因果、人脉与探索展开的修行模拟 | [`xx3.1.html`](./xx3.1.html) |

## 本地运行

直接双击 `index.html` 即可浏览。若浏览器限制本地文件的部分功能，可在仓库目录启动一个静态服务器：

```bash
python -m http.server 8000
```

然后打开 <http://localhost:8000>。

## GitHub Pages 部署

仓库已包含 `.github/workflows/pages.yml`。推送到 `main`（或 `master`）后，GitHub Actions 会自动发布站点：

1. 将本目录内容推送到 GitHub 仓库。
2. 在仓库 **Settings → Pages** 中将 **Source** 设为 **GitHub Actions**。
3. 等待 `Deploy to GitHub Pages` 工作流完成，在 Actions 日志中打开站点地址。

如果默认分支不是 `main` 或 `master`，请编辑工作流中的 `branches` 列表。

## AI Key 安全说明

API Key 只在游戏页面中保存在浏览器 `localStorage`，不会被提交到 GitHub。不要把真实 Key 写进 HTML、README、Issue 或截图；公开分享时建议使用临时 Key 并设置额度限制。

## 自定义 GitHub 链接

首页的 GitHub 按钮指向本项目仓库：<https://github.com/achengz/AI-driven-text-based-game>。

## 许可

如需公开复用，建议在仓库中添加 MIT License；其中使用的模型、字体或第三方素材请遵循各自许可。
