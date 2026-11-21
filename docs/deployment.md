# 独立讲义站迁移记录

## 当前状态

讲义的正式阅读入口已统一为 [blog.annouimo.com/notes](https://blog.annouimo.com/notes/)，由 [Annouimo/annouimo-publishing](https://github.com/Annouimo/annouimo-publishing) 构建。该工程通过 `notes.lock` 固定本仓库的讲义与组件版本。

2026-11-22，Cloudflare 已将 `learn.annouimo.com` 从 `why-notes` Worker 解绑，并移除对应 DNS 记录。Worker 与本仓库均保留；此后不再通过该子域名访问讲义。

## 历史记录

2026-11-14，独立 Astro 站点首次部署到 Cloudflare Workers Static Assets。部署流程曾使用 Cloudflare Workers Builds，Node.js 24，并以 `npm run check` 验证；早期生产构建仅包含首页，讲义保持草稿。其后讲义源稿迁入博客发布工程，博客生产站已提供一致连续与麦克斯韦两篇讲义。

本文件仅记录独立站时期的部署背景。若需更新正式讲义，请在 annouimo-notes 修改源稿后，按 annouimo-publishing 的发布流程生成并检查博客预览。
