# n8n

## 工作流简介

本工作流通过 Jina.ai 实现对指定网站的批量抓取，无需 API Key。主要流程如下：

1. **手动触发**：通过“Test workflow”按钮启动流程。
2. **设置网站 Sitemap URL**：配置需要抓取的网站 sitemap 地址。
3. **获取并解析 Sitemap**：自动请求 sitemap，解析出所有页面 URL。
4. **筛选页面**：可根据主题或关键词过滤需要抓取的页面。
5. **批量抓取页面内容**：循环遍历每个页面，调用 Jina.ai Web Scraper 获取内容。
6. **提取标题与 Markdown 内容**：自动从抓取结果中提取标题和 Markdown 格式正文。
7. **保存为 Markdown 文件**：将每个页面内容保存为本地 Markdown 文件，也可同步到 Google Drive。

> 适用于需要批量归档、备份或分析网站内容的场景。请合理使用，遵守相关法律法规。