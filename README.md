# AutoJsPro 可复建交付

建议将 GitHub 仓库设为 Private。`release-assets/` 内两个大文件作为 GitHub Release 附件上传，不提交进普通 Git 历史；工程 ZIP 超过 GitHub 单文件大小限制。

- `release-assets/AutoJsPro_freshkey_279a.apk`：Android 35 / ARM64 模拟器实测的新签名 APK。
- `release-assets/AutoJsPro_current_buildkit.zip`：可修改、可重建的工程包。
- `FINAL_ACCEPTANCE.md`：实测范围和未完成项。
- `SHA256SUMS.txt`：发布附件哈希。

APK 使用新的开发签名，不能覆盖官方签名安装。卸载旧包前请备份应用数据。工程仍含原 DEX/native 和 214 个预编译恢复类，不是完整原厂源码。其它限制见验收记录。
