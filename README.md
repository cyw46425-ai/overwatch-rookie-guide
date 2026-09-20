# OW 助手｜守望先锋新手助手

面向《守望先锋》新手玩家的静态 Web 助手，提供智能问答、英雄数据、知识百科、活动资讯、版本改动、赛事与视频直播入口。

## 在线预览

https://overwatch-rookie-guide.cyw46425.chatgpt.site

## 项目结构

```text
dist/
├─ index.html          页面入口
├─ styles.css          页面样式与动效
├─ app.js              交互、检索与上下文逻辑
├─ heroes-data.js      英雄数据
├─ knowledge.js        本地知识库
└─ assets/             英雄、地图、资讯与视频图片
```

## 本地运行

项目无需构建。请在项目根目录运行静态文件服务器：

```bash
python -m http.server 8080 --directory dist
```

然后访问 `http://localhost:8080`。

## 发布到 GitHub Pages

仓库内已包含 `.github/workflows/pages.yml`。将代码推送到 `main` 分支后，在 GitHub 仓库的 **Settings → Pages → Build and deployment → Source** 中选择 **GitHub Actions**，工作流会自动发布 `dist/`。

## 数据说明

- 英雄、地图、活动、赛事和视频信息来自项目内置知识库与外部链接。
- 胜率、版本与活动信息具有时效性，正式发布前应再次核对来源和日期。
- 本项目为非官方玩家工具，与 Blizzard Entertainment 无隶属关系。

