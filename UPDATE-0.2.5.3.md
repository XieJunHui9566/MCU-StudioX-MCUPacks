# IDE 0.2.5.3 配套说明

[MCU StudioX 0.2.5.3](https://github.com/XieJunHui9566/MCU-StudioX/releases/tag/v0.2.5.3) 新增 OpenOCD 变量绘图和中英双语诊断，并完善工程编辑与内置 Agent。本次不修改器件实现，公开目录仍为 62 个 StudioX Pack 格式 1 包，所有 `.mcupack`、索引和 SHA-256 保持不变。

RP2040 / RP2350 保持 0.2.0，提供 C SDK 和 MicroPython 模板。STM32 HAL、Puya、GD32 等现有公开修订继续使用，不回退版本、不恢复过时文件。已安装这些包的用户无需重复下载；新安装用户可在 IDE 中同步目录，或下载 Release 中的公开器件包合集。

OpenOCD 绘图复用已配置的调试会话，运行中读取能力取决于芯片、探针和调试后端。本版完成离线验证，尚未完成实板采样验收；这项 IDE 功能不改变各器件包原有的硬件验证状态。

各包来源与再分发范围见 [第三方声明](THIRD_PARTY_NOTICES.md)，具体文件摘要见 [SHA256SUMS.txt](SHA256SUMS.txt)。
