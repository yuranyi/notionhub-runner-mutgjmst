# NotionHub Runner

这个仓库由 NotionHub 自动创建，用于运行已配置同步服务的 GitHub Actions。

- 新仓库默认创建为 public；已有私有仓库不会被自动公开。
- 敏感信息只写入 Repository Secrets，不会出现在仓库文件中。
- 仅为已启用且配置完整的付费或免费服务生成 workflow。
- 免费开源 workflow 运行时不请求 NotionHub Worker。
- 支持媒体的服务会在同一次 workflow 中先同步数据，再下载上传图片和大文件。
- workflow 由 NotionHub 自动更新，手动修改可能会在下次同步时被覆盖。
