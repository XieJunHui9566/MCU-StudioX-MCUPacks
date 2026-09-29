# MCU StudioX 器件包

2026-09-30：新增 **272 个 ARM32 器件包 / 2,777 个器件条目**。公开目录现有 **334 包**，其中 **325 个 ARM32 包 / 3,453 个器件条目**。原有 62 包内容、版本及校验值未改变；IDE 保持 **0.2.5.3**。详见 [本轮更新说明](UPDATE-ARM32-2026-09-30.md)、[新增包清单](ARM32-PACKS-2026-09-30.md) 和 [ARM32 整包下载](https://github.com/XieJunHui9566/MCU-StudioX-MCUPacks/releases/tag/arm32-2026-09-30)。

这里按芯片品牌存放 [MCU StudioX](https://github.com/XieJunHui9566/MCU-StudioX) 的 `.mcupack` 器件包。原有目录收录 16 个普冉 PY32 包、2 个 Raspberry Pi RP2040 / RP2350 包、23 个 STM32 HAL 包、13 个 GD32 包、7 个 Espressif 包及 1 个 STC 包，共 **62 个**；本轮另增 272 包，全部采用 StudioX Pack **格式 1**。器件包保留各自独立版本号。每个包 ID 只保留当前可公开的最新版本。

此前 0.2.5.2 配套更新新增 RP2040 并更新 RP2350，两包均为 0.2.0，提供 C SDK 与 MicroPython 模板。已有 STM32 HAL、Puya 和 GD32 的公开修订保持不变；旧 RP2350 文件由新版替代，Git 历史保留。详见[0.2.5.2 更新](UPDATE-0.2.5.2.md)及[第三方来源](THIRD_PARTY_NOTICES.md)。

| 品牌 | 器件包 | 版本 | 收录范围 | 验证状态 |
| --- | --- | --- | --- | --- |
| 普冉 Puya | [PY32F002A](Puya/puya.py32f002a-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F002B](Puya/puya.py32f002b-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F003](Puya/puya.py32f003-0.1.1.mcupack) | 0.1.1 | 3 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F005](Puya/puya.py32f005-0.1.2.mcupack) | 0.1.2 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F030](Puya/puya.py32f030-0.1.1.mcupack) | 0.1.1 | 4 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F031](Puya/puya.py32f031-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F032](Puya/puya.py32f032-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F033](Puya/puya.py32f033-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F040](Puya/puya.py32f040-0.1.2.mcupack) | 0.1.2 | 4 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F071](Puya/puya.py32f071-0.1.2.mcupack) | 0.1.2 | 4 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F072](Puya/puya.py32f072-0.1.2.mcupack) | 0.1.2 | 4 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F090](Puya/puya.py32f090-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F092](Puya/puya.py32f092-0.1.1.mcupack) | 0.1.1 | 1 个容量型号 | 离线编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F403](Puya/puya.py32f403-0.1.0.mcupack) | 0.1.0 | 11 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F410](Puya/puya.py32f410-0.1.0.mcupack) | 0.1.0 | 6 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| 普冉 Puya | [PY32F420](Puya/puya.py32f420-0.1.0.mcupack) | 0.1.0 | 2 个完整料号 | 工程创建和代表型号编译通过；尚无实板测试 |
| Raspberry Pi | [RP2040](Raspberry-Pi/raspberrypi.rp2040-0.2.0.mcupack) | 0.2.0 | RP2040；C SDK、MicroPython | C 工程真实编译、MicroPython 离线检查通过；尚无 RP2040 实板验收 |
| Raspberry Pi | [RP2350](Raspberry-Pi/raspberrypi.rp2350-0.2.0.mcupack) | 0.2.0 | RP2350A；C SDK、MicroPython | C 编译和既有兼容板验证；MicroPython 工程与编辑、传输离线检查通过 |
| STMicroelectronics | [STM32F100](STMicroelectronics/studiox.stm32f100-0.1.2.mcupack) | 0.1.2 | 19 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F101](STMicroelectronics/studiox.stm32f101-0.1.2.mcupack) | 0.1.2 | 29 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F102](STMicroelectronics/studiox.stm32f102-0.1.2.mcupack) | 0.1.2 | 8 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F103](STMicroelectronics/studiox.stm32f103-0.1.2.mcupack) | 0.1.2 | 29 个基础型号；HAL、HAL + FreeRTOS | F103C8 两模板真实编译通过；其他型号与实板尚未验收 |
| STMicroelectronics | [STM32F105](STMicroelectronics/studiox.stm32f105-0.1.2.mcupack) | 0.1.2 | 6 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F107](STMicroelectronics/studiox.stm32f107-0.1.2.mcupack) | 0.1.2 | 4 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F401](STMicroelectronics/studiox.stm32f401-0.1.2.mcupack) | 0.1.2 | 12 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F405](STMicroelectronics/studiox.stm32f405-0.1.2.mcupack) | 0.1.2 | 5 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F407](STMicroelectronics/studiox.stm32f407-0.1.2.mcupack) | 0.1.2 | 6 个基础型号；HAL、HAL + FreeRTOS | F407ZG 两模板真实编译通过；其他型号与实板尚未验收 |
| STMicroelectronics | [STM32F410](STMicroelectronics/studiox.stm32f410-0.1.2.mcupack) | 0.1.2 | 6 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F411](STMicroelectronics/studiox.stm32f411-0.1.2.mcupack) | 0.1.2 | 6 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F412](STMicroelectronics/studiox.stm32f412-0.1.2.mcupack) | 0.1.2 | 8 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F413](STMicroelectronics/studiox.stm32f413-0.1.2.mcupack) | 0.1.2 | 10 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F415](STMicroelectronics/studiox.stm32f415-0.1.2.mcupack) | 0.1.2 | 4 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F417](STMicroelectronics/studiox.stm32f417-0.1.2.mcupack) | 0.1.2 | 6 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F423](STMicroelectronics/studiox.stm32f423-0.1.2.mcupack) | 0.1.2 | 5 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F427](STMicroelectronics/studiox.stm32f427-0.1.2.mcupack) | 0.1.2 | 8 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F429](STMicroelectronics/studiox.stm32f429-0.1.2.mcupack) | 0.1.2 | 17 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F437](STMicroelectronics/studiox.stm32f437-0.1.2.mcupack) | 0.1.2 | 7 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F439](STMicroelectronics/studiox.stm32f439-0.1.2.mcupack) | 0.1.2 | 11 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F446](STMicroelectronics/studiox.stm32f446-0.1.2.mcupack) | 0.1.2 | 8 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F469](STMicroelectronics/studiox.stm32f469-0.1.2.mcupack) | 0.1.2 | 18 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| STMicroelectronics | [STM32F479](STMicroelectronics/studiox.stm32f479-0.1.2.mcupack) | 0.1.2 | 12 个基础型号；HAL、HAL + FreeRTOS | 代表组合两模板编译通过；尚无实板验收 |
| Espressif | [ESP32-WROOM-32](Espressif/espressif.esp32-wroom-32-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP32-C3](Espressif/espressif.esp32c3-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP32-C5](Espressif/espressif.esp32c5-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP32-C6](Espressif/espressif.esp32c6-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP32-P4](Espressif/espressif.esp32p4-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP32-S3](Espressif/espressif.esp32s3-0.1.1.mcupack) | 0.1.1 | ESP-IDF 5.5.4；官方 Hello World、FreeRTOS 示例 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| Espressif | [ESP8266](Espressif/espressif.esp8266-0.1.0.mcupack) | 0.1.0 | ESP8266 RTOS SDK 3.4.0；原生应用模板 | 原生 SDK 构建入口；具体板卡与 Flash/PSRAM 由工程配置 |
| GigaDevice | [GD32C10X](GigaDevice/gigadevice.gd32c10x-0.1.0.mcupack) | 0.1.0 | 4 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32E10X](GigaDevice/gigadevice.gd32e10x-0.1.0.mcupack) | 0.1.0 | 8 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32E23X](GigaDevice/gigadevice.gd32e23x-0.1.0.mcupack) | 0.1.0 | 15 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32E50X](GigaDevice/gigadevice.gd32e50x-0.1.0.mcupack) | 0.1.0 | 24 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F10X](GigaDevice/gigadevice.gd32f10x-0.1.0.mcupack) | 0.1.0 | 106 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F1X0](GigaDevice/gigadevice.gd32f1x0-0.1.0.mcupack) | 0.1.0 | 41 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F20X](GigaDevice/gigadevice.gd32f20x-0.1.0.mcupack) | 0.1.0 | 27 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F30X](GigaDevice/gigadevice.gd32f30x-0.1.1.mcupack) | 0.1.1 | 40 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F3X0](GigaDevice/gigadevice.gd32f3x0-0.1.1.mcupack) | 0.1.1 | 36 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F403](GigaDevice/gigadevice.gd32f403-0.1.1.mcupack) | 0.1.1 | 15 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32F4XX](GigaDevice/gigadevice.gd32f4xx-0.1.1.mcupack) | 0.1.1 | 60 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32L23X](GigaDevice/gigadevice.gd32l23x-0.1.0.mcupack) | 0.1.0 | 8 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| GigaDevice | [GD32VF103](GigaDevice/gigadevice.gd32vf103-0.1.0.mcupack) | 0.1.0 | 14 个容量/封装基础型号；标准外设库 | 离线工程与编译适配；尚无实板验收 |
| STC | [STC 8 位系列](STC/stc.stc8-0.1.0.mcupack) | 0.1.0 | 24 个明确型号；STC89、STC12、STC15、STC8G、STC8H | SDCC 工程；原厂头文件不再分发，仅保留重新生成的 SFR 定义 |

在 MCU StudioX 的器件包管理界面导入所需的 `.mcupack`，再按目标芯片或板卡新建工程。器件包不包含编译器或调试器可执行文件，构建还需 IDE 配套工具链。每个包内的 `manifest.json` 列出具体型号、模板和工具要求，`README.md` 说明使用范围，`provenance.json` 或 `vendor/provenance.json` 记录 SDK 来源与校验信息。Espressif 包引用 IDE 的共享 SDK；包本身不含完整 ESP-IDF/ESP8266 SDK。

PY32 共有 27 个 F0 容量型号和 19 个 F4 完整料号。新增 13 个 F0 包已通过项目校验器的 **81 次工程创建和 81 次真实编译**，没有访问硬件。PY32 的实板下载和调试尚未验收，这些包没有声明下载或调试目标。RP2040 / RP2350 包针对外部 12 MHz 晶振、4 MiB QSPI Flash 的 RP2350A 板型；实板结果不能推广到其他 RP2350 板型、RISC-V 内核或 Pico 2 W。

F005/F040/F071/F072 的 0.1.2 版与 F031/F032/F033/F090/F092 的 0.1.1 版仅补入 Arm CMSIS 所需的 Apache-2.0 许可正文并更新包版本和校验索引；原厂 SDK 源文件、器件参数与构建配置未改动。版本号提升使已导入旧版的用户可并存安装。

STM32 的 23 个 HAL-only 包共覆盖 244 个基础型号，只含来自 ST 官方 STM32CubeF1/F4 的 CMSIS、HAL、启动文件及 FreeRTOS 10.3.1（FreeRTOS 来自 STM32CubeF4），不含 SPL、Keil DFP 源文件或工具链二进制。23 包均完成 StudioX 完整导入及逐文件哈希校验；244 个型号的 Flash/RAM/CCM 链接配置、启动文件与模板引用通过静态检查。新增 21 个子系列按 HAL 宏、启动文件和时钟配置选取代表型号，并覆盖最小 RAM 与最大 Flash 边界，两种模板共 106 组真实编译通过；F103C8 和 F407ZG 两模板另有 4 组真实编译通过，合计 110 组，均生成 ELF/BIN/HEX。此验证不代表全部型号逐一编译，也不代表实板下载或调试已验收。

## IDE 在线同步

IDE 可以从本仓库的 [index.json](index.json) 获取公开器件包目录，比较本地已安装的包，只下载新增或更新的 `.mcupack`，校验 SHA-256 后再自动导入。索引的 `formatVersion` 表示目录格式；每个 `packs` 条目包含仓库相对路径 `path`、包标识 `id`、版本 `version`、文件校验值 `sha256` 和字节数 `size`。`id`、`version` 取自包内的 `manifest.json`，校验值与 [SHA256SUMS.txt](SHA256SUMS.txt) 一致。下载与索引应固定在同一仓库提交上，避免同步期间分支更新造成版本不一致。

在线目录只收录已完成来源及再分发许可核查的器件包；其他本地包不会因 IDE 同步而上传到此仓库。SHA-256 用于检查下载文件的完整性，包内源码仍遵循各自的第三方许可。

文件 SHA-256 见 [SHA256SUMS.txt](SHA256SUMS.txt)。第三方来源与许可见 [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) 及各包内的许可证和源码声明。目录公开并不改变第三方文件原有许可。
