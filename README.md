# AI-driven-text-based-game

我的个人浏览器游戏分享站，收录 AI 驱动的互动叙事和文字游戏实验。项目包含武侠冒险模拟、现代人生模拟与修仙主题 RPG，打开网页即可游玩，无需安装额外运行时。

## Online

部署后访问：`https://achengz.github.io/AI-driven-text-based-game/`

首页：[`index.html`](./index.html)

## Games

| Game | Description | Entry |
| --- | --- | --- |
| 江湖风云模拟 | 古风开放世界文字 RPG，支持 NPC 关系、记忆、背包、存档和 AI 对话 | [`wuxia.html`](./wuxia.html) |
| 现代人生模拟 | 以工作、关系和城市生活为主题的互动人生故事 | [`modern-life.html`](./modern-life.html) |
| 修仙问道模拟 | 围绕功法、因果、人脉与探索展开的修行模拟 | [`cultivation.html`](./cultivation.html) |

三个游戏使用统一的自定义 OpenAI 兼容接口配置：玩家自行填写接口地址、模型 ID 与 API Key。项目不内置中转站、官方模型或默认密钥。

## Local development

直接双击 `index.html` 即可浏览。若浏览器限制本地文件的部分功能，可在仓库目录启动静态服务器：

```bash
python -m http.server 8000
```

然后打开 <http://localhost:8000>。

## GitHub Pages

仓库已包含 `.github/workflows/pages.yml`。推送到 `main` 后，GitHub Actions 会自动发布站点：

1. 在仓库 **Settings → Pages** 中将 **Source** 设为 **GitHub Actions**。
2. 等待 `Deploy to GitHub Pages` 工作流完成。
3. 访问 <https://achengz.github.io/AI-driven-text-based-game/>。

## API key safety

API Key 只在游戏页面中保存在浏览器 `localStorage`，不会被提交到 GitHub。不要把真实 Key 写进 HTML、README、Issue 或截图；公开分享时建议使用临时 Key 并设置额度限制。

## License

项目许可见 [`LICENSE`](./LICENSE)。其中使用的模型、字体或第三方素材请遵循各自许可。
