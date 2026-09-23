# MCU StudioX 器件包

这里按芯片品牌存放 [MCU StudioX](https://github.com/XieJunHui9566/MCU-StudioX) 的 `.mcupack` 器件包。当前公开目录仅收录已核对来源、第三方许可和包内容的 StudioX Pack **格式 1** 包。

| 品牌 | 器件包 | 版本 | 收录范围 | 验证状态 |
| --- | --- | --- | --- | --- |
| 普冉 Puya | [PY32F403](Puya/puya.py32f403-0.1.0.mcupack) | 0.1.0 | 11 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F410](Puya/puya.py32f410-0.1.0.mcupack) | 0.1.0 | 6 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F420](Puya/puya.py32f420-0.1.0.mcupack) | 0.1.0 | 2 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| Raspberry Pi | [RP2350](Raspberry-Pi/raspberrypi.rp2350-0.1.0.mcupack) | 0.1.0 | RP2350A、Pico 2 / 相同配置的兼容板 | C 工程编译及一块 Pico 2 兼容板的下载、调试已验证 |

在 MCU StudioX 的器件包管理界面导入所需的 `.mcupack`，再按目标芯片或板卡新建工程。器件包不包含编译器或调试器可执行文件，构建还需 IDE 配套工具链。每个包内的 `manifest.json` 列出具体型号、模板和工具要求，`README.md` 说明使用范围，`provenance.json` 记录 SDK 来源与校验信息。

PY32 的实板下载和调试尚未验收，因此这三个包没有声明下载或调试目标。RP2350 包针对外部 12 MHz 晶振、4 MiB QSPI Flash 的 RP2350A 板型；实板结果不能推广到其他 RP2350 板型、RISC-V 内核或 Pico 2 W。

文件 SHA-256 见 [SHA256SUMS.txt](SHA256SUMS.txt)。第三方来源与许可见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) 及各包内的许可证和源码声明。目录公开并不改变第三方文件原有许可。
