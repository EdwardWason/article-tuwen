# Changelog

## v1.1.0 — 2026-07-15

### Security Audit Fixes (ClawHub SkillSpector)

- **端口定向清理**：将"杀全部Python进程的旧命令"替换为基于 `Get-NetTCPConnection -LocalPort 8090` 的定向清理（仅终止占用8090端口的进程）
- **云上传consent gate**：飞书云盘同步从自动执行改为需用户确认，Phase 4.2添加确认门
- **隐私声明**：SKILL.md/README.md/README_EN.md 添加"数据处理与隐私"章节
- **触发边界**：添加明确触发条件和不触发条件
- **移除explorer.exe**：不再自动打开文件夹，仅告知输出路径
- **权限声明**：添加5维度权限声明表格
- **description更新**：添加"Cloud sync is opt-in only"

### Architecture

- Phase 1改为调用transcript-crafter完整8步流程（含5工具搜索补充）
- 字号铁律升级：正文≥32px，辅助≥28px，元信息≥24px

## v1.0.0 — 2026-06-14

### Initial Release

- One-shot pipeline: 素材 → 长文 → 5-9张社交卡片 + 文字稿
- 编排层架构：调度transcript-crafter + xhs-crafter
- 多样性轮换：8封面词 + 8封底词 + 5主题池
- 截图安全检查
- 桌面 + 飞书云盘双通道交付
