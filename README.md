# Raycast macOS 简体中文汉化 · 2.7.3.0 arm64

为 **Raycast 2.7.3.0 · Apple Silicon（M 系列 Mac）** 提供非官方简体中文资源补丁。
本版参考 [zwjtano/raycast-macos-zh-CN](https://github.com/zwjtano/raycast-macos-zh-CN) 的 2.7.2.0 汉化包迁移；原译文及插件显示转换代码来源于原包。本仓库维护 2.7.3.0 适配与验证，不声称原译文均由本仓库作者创作。

**[下载汉化包](https://github.com/ZIKmars/raycast-macos-zh-CN/releases/latest)** · [插件清单](docs/插件清单.md) · [验证报告](docs/验证报告.json)

## 支持范围

| 项目 | 说明 |
| --- | --- |
| 系统与架构 | macOS，Apple Silicon / arm64 |
| Raycast 版本 | 仅 2.7.3.0；校验主程序及资源 SHA-256 |
| 资源文件 | 200 个 |
| 界面 | 主搜索、设置及部分操作提示 |
| 插件 | 沿用原包商店前十页 100 个插件及 Mole 的部分显示文案 |
| 完整汉化 | 否；菜单栏、部分动态内容和主搜索输入提示仍为英文 |
| 备份与还原 | 安装前备份，提供恢复工具 |

插件范围来自原包 2026-09-21 商店排序快照，不是实时排名，也不代表全部插件内部功能均已验收。

## 安装

1. 确认已安装并正常打开过官方 **Raycast 2.7.3.0 arm64**，默认路径 `/Applications/Raycast.app`。
2. 从 Releases 下载 `Raycast-2.7.3.0-arm64-汉化包.zip`，完整解压。
3. 从 Raycast 菜单 **Quit Raycast** 完全退出。
4. 双击 **安装汉化.command**，回车使用默认路径，再确认安装。
5. 安装结束后打开 Raycast。

不需要 Python、Node 或开发环境。**GitHub 的 Source code ZIP 不是安装包**；仓库中的 installer 文件只供审阅，必须使用 Release 中含 payload 的完整包。

## 恢复与更新

完全退出 Raycast，双击同一汉化包的 **恢复原版.command**。
备份位于 `~/Library/Application Support/Raycast-Chinese-Patch/2.7.3.0/`。保留备份和补丁包，不要移动已打补丁的应用。

**更新前先恢复原版，更新后使用匹配新版本的汉化包。** 本补丁不能跨版本使用；应用更新或资源被其他工具修改后，恢复工具会拒绝覆盖。

## 已验证与边界

- 200 个资源文件的 JavaScript 语法及模块引用检查通过。
- 本机安装后 200 个资源文件与最终补丁指纹一致。
- 本机回滚两次，恢复后完整官方签名检查通过。
- 实际打开验证：主搜索无错误页、通用设置中文与布局正常、商店欢迎说明页中文正常。
- 未代为接受商店服务条款，未逐一验收插件内部流程、登录后页面或其他机器的启动情况。

本包只修改资源，不修改原生可执行文件、账户或用户数据库，不重新签名、不关闭系统保护。**资源修改会使完整官方签名校验失效，其他机器可能被 macOS 拦截。** 若出现启动问题，优先恢复原版；不要关闭全局系统保护或重置数据库。

## 来源与许可

- Raycast 应用与相关名称归原权利人所有，本项目不是 Raycast 官方中文版，不包含官方应用安装程序。
- 2.7.2.0 译文及插件显示转换代码：来自 [zwjtano/raycast-macos-zh-CN](https://github.com/zwjtano/raycast-macos-zh-CN) 发布的汉化包。
- 保留原包 Acorn、Unicode 许可与来源记录，见 `docs/` 及安装包对应文件。
- 不对第三方资源附加不明的统一开源许可；转载和派生使用需遵循各自原有许可。

版本适配日期：2026-10-10。
