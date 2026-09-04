<div align="center">

<img src="assets/img/logo.png" width="170" alt="ExifMate">

# ExifMate

**照片和视频的元数据，一眼看清、批量修好、改错可撤。**

完全离线的 EXIF 查看 / 修复 / 批量修改工具（Windows）

**🛡️ 完全离线 &nbsp;·&nbsp; 🔄 历史终身可回溯 &nbsp;·&nbsp; 🎬 独家视频支持 &nbsp;·&nbsp; ⚡ 多线程高速 &nbsp;·&nbsp; 📅 时间批量修复 &nbsp;·&nbsp; 🕐 时间戳回写 &nbsp;·&nbsp; ✏️ 模板化重命名**

`Windows 10 / 11` · `免费版 + 完整版`

[官网 exifmate.com](https://exifmate.com) · [从微软商店下载](https://apps.microsoft.com/search?query=ExifMate) · [隐私政策](https://exifmate.com/privacy/) · [问题反馈](https://github.com/zm1107/exifmate/issues)

☕ 觉得好用？[请作者喝杯咖啡](#请作者喝杯咖啡)

<!-- TODO: 上架后替换为正式商店商品页链接，并在此处放一张主界面截图 -->

</div>

<p align="center"><b>简体中文</b> · <a href="README.en.md">English</a></p>

## 它能帮你解决什么

| 你遇到的麻烦 | ExifMate 的答案 |
|---|---|
| 相机时间没调 / 时区错，几千张照片日期全错 | 批量偏移或精确设置拍摄时间，文件时间戳一并对齐 |
| 老照片、扫描件没有日期，永远排不到正确位置 | 文件名智能识别自动回写缺失日期，RAW+JPG 配对互相补全 |
| 想批量改元数据，只找到 ExifTool 命令行教程 | 图形界面覆盖 ExifTool 全部能力，任意标签可视化批量写入 |
| 批量改完才发现改错，普通工具没有"后悔药" | 每次操作入库快照，任意一步 / 任意一批一键恢复 |
| 视频（手机 / 无人机）的元数据没人管 | 原生支持 MP4 / MOV / MKV / MTS 等十余种视频格式 |
| 发圈 / 交付前担心照片泄露位置 | 一键清除 GPS 与设备序列号，或批量写入版权作者信息 |

## 功能特性

- **看得全**：分组树形展示全部元数据，修改前后差异对比高亮，RAW 内嵌 JPEG 预览、视频内嵌播放
- **全流程多线程**：哈希、EXIF 读取、批量写入、重命名各自独立线程池并行执行，大批量文件处理依然流畅
- **改错可恢复，历史终身可回溯**：全部操作写入本地记录库永久保存（含文件哈希与操作前后快照），跨会话不丢失，任意一步、任意历史批次随时一键还原
- **时间戳回写**：以拍摄日期（或从文件名识别出的日期）批量回写文件的**创建时间与修改时间**（Windows 创建时间走系统 API），资源管理器排序、备份归档立即归位
- **模板化批量重命名**：按拍摄日期、相机型号、批内序号、原名、扩展名自由组合输出模板（如 `{Y4}{M2}{D2}_{h}{m}{s}_{相机型号}`），同秒多张自动追加 `_01/_02` 序号，重命名前完整预览
- **智能识别**：文件名识别占位符语法（`{Y4}{M2}{D2}_{h}{m}{s}`、通配符 `{seg}` `{*}`），多模板按自定义顺序匹配，首个命中生效
- **完全离线**：零联网、零账号、零遥测——隐私不是承诺，是架构

**支持格式**：JPEG / PNG / GIF / BMP / TIFF / WebP / HEIC；CR2 / CR3 / NEF / NRW / ARW / RAF / PEF / SRW / DNG 等主流 RAW；MP4 / M4V / MOV / AVI / MKV / WMV / FLV / WebM / MTS / M2TS / MOD / MPG 等视频。

## 免费版与完整版

| | 免费版 | 完整版 |
|---|---|---|
| 全部功能 | ✓ | ✓ |
| 单次批量处理文件数 | ≤ 10 个 | 不限 |
| 优先技术支持 | — | ✓ |
| 价格 | 免费 | 一次性买断 |

完整版在微软商店内购买，价格以[商店页面](https://apps.microsoft.com/search?query=ExifMate)为准，1.x 版本免费更新。

## 隐私

ExifMate **完全离线运行**：应用代码不含任何网络访问功能，不收集任何个人信息，你处理的照片和视频始终留在你自己的电脑上。详见[隐私政策](https://exifmate.com/privacy/)。

## 反馈与支持

- 🐛 Bug 与功能建议：[GitHub Issues](https://github.com/zm1107/exifmate/issues)（推荐，中英文均可）
- 📧 邮件：dev@exifmate.com

## 关于本仓库

本仓库托管 ExifMate 官方网站（exifmate.com）的源码；应用本身为闭源分发，基于 [ExifTool](https://exiftool.org)（Artistic License 2.0）等开源组件构建，许可声明随软件分发。

## 致谢

ExifMate 站在以下优秀开源项目的肩膀上，向原作者与开源社区致以诚挚谢意：

| 项目 | 用途 | 许可证 | 主页 |
|---|---|---|---|
| [ExifTool](https://exiftool.org) | EXIF / XMP / QuickTime 元数据读写核心 | Artistic License 2.0 | Copyright 2003-2026, Phil Harvey |
| [Qt / PySide6](https://www.qt.io) | 图形界面框架 | LGPL-3.0 | Qt Company |
| [Pillow](https://python-pillow.org) | 图像解码与预览 | MIT-CMU | Python Pillow 社区 |
| [pillow-heif](https://github.com/bigcat88/pillow_heif) | HEIC / HEIF 格式支持 | MIT | bigcat88 |
| [xxHash](https://github.com/Cyan4973/xxHash) | 文件哈希（恢复校验） | BSD-2-Clause | Yann Collet |
| [SQLite](https://www.sqlite.org) | 本地操作记录数据库 | Public Domain | SQLite 开发者 |
| [Python](https://www.python.org) | 运行时 | PSF License | Python 软件基金会 |
| [cryptography](https://github.com/pyca/cryptography) | 程序完整性校验签名 | Apache-2.0 | pyca |

感谢所有开源贡献者——你们让独立开发者也能造出专业级的工具。

## 请作者喝杯咖啡

如果 ExifMate 帮到了你，欢迎请作者喝杯咖啡 ☕——你的支持就是持续更新的动力。

<p align="center">
  <img src="assets/img/coffee-wx.jpg" alt="微信收款码" width="260">
</p>

> 微信「扫一扫」上方收款码即可支持，金额随意，心意最重要。
