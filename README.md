# android-emulator-probe

Phase 0 探针仓库：验证 GitHub Actions Linux runner 能否正常 boot 安卓模拟器。

- **与 luxp1990 其他仓库零关联**（独立仓库、独立 Actions 历史、公共仓库不占私有额度池）
- 配置 = pachli-android 防坑六件套（简化版），防 2026-06 runner 挂起坑（ReactiveCircus #478）
- 触发：push 到 main 自动跑 / Actions 页面手动触发
- 证据：run 日志 + 模拟器首屏截图（artifact `probe-evidence`）
- 成功标准：日志出现 `PROBE_OK` + 截图非空

仅含本 workflow，无任何业务代码。
