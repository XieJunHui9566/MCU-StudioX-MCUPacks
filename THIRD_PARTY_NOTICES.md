# 第三方来源与许可

本仓库是器件包的分发目录，不对包内所有源码统一授予一种开源许可。使用或再分发某个包时，应遵守该包中原有的版权声明和许可。以下列出原有 62 包及本轮新增 272 包的主要来源；逐文件来源及哈希见包内 `provenance.json`。

## Puya：PY32F0、PY32F403、PY32F410、PY32F420

16 个包采用 [OpenPuya 社区镜像](https://github.com/OpenPuya)中的固件源码。OpenPuya 不是普冉官方代码仓库。型号、封装和容量另外按普冉产品资料核对；这些包不代表普冉官方发布或认可。每个包的 `provenance.json` 记录具体镜像、提交和源文件哈希。

PY32F0 包内保留 `licenses/Puya-BSD-3-Clause.txt`；含 Apache-2.0 CMSIS 文件的 9 个修订包还保留 `licenses/CMSIS-LICENSE.txt`。F002A/F002B/F003/F030 的 Arm CMSIS 文件使用源文件中完整保留的 BSD 许可声明，无需另附 Apache 许可。PY32F403/F410/F420 包内保留 `licenses/OpenPuya-BSD-3-Clause.txt` 与 `licenses/CMSIS-LICENSE.txt`（Apache-2.0）。Puya、STMicroelectronics、OpenPuya 和 Arm 源文件中的原版权声明均保留。具体文件适用其自身声明的许可；请勿把仓库说明或其他项目的许可覆盖到这些第三方文件。

## Raspberry Pi：RP2040、RP2350

两个包的 SDK 来源是 [Raspberry Pi Pico SDK 2.2.0](https://github.com/raspberrypi/pico-sdk/tree/2.2.0)。包内 `sdk/LICENSE.TXT` 保留 SDK 的 BSD-3-Clause 许可。`sdk/src/rp2_common/pico_printf/` 下的第三方 printf 源文件另在文件头保留完整 MIT 许可和作者声明。

MicroPython 模板和 API 提示由 StudioX 生成，固件通过官方页面单独获取；包内没有 MicroPython 解释器固件。原有 C SDK 许可和逐文件来源记录继续保留。

## STMicroelectronics：STM32F1、STM32F4

23 个 0.1.2 包的 CMSIS/CMSIS Device、HAL 与启动文件分别来自 ST 官方 [STM32CubeF1 v1.8.7](https://github.com/STMicroelectronics/STM32CubeF1/tree/v1.8.7) 和 [STM32CubeF4 v1.28.3](https://github.com/STMicroelectronics/STM32CubeF4/tree/v1.28.3)；FreeRTOS 10.3.1 来自后者。包内 `licenses/` 保留 CMSIS/CMSIS Device 的 Apache-2.0、ST HAL 的 BSD-3-Clause、FreeRTOS 的 MIT 许可及 STM32Cube 软件清单，源码原版权声明未改。`provenance.json` 列有收入包中的每个 SDK 文件 SHA-256。包内没有 SPL 或 Keil DFP 的器件头文件，也没有工具链二进制；请勿把仓库自身许可证套用到这些第三方组件。

这些第三方商标只用于说明器件兼容性，不表示相应厂商为本仓库背书。


## Espressif：ESP32、ESP32-P4/S3/C3/C5/C6、ESP8266

6 个 ESP32 目标引用 [ESP-IDF v5.5.4](https://github.com/espressif/esp-idf/tree/v5.5.4)。包中的 Hello World、FreeRTOS 示例保留原文件的 CC0/公共领域声明，并保留上游 `LICENSE`（Apache-2.0）；各示例的来源与内容校验值记录在 `provenance.json`。包不含 IDF SDK、工具链、Python 或其第三方组件。

ESP8266 包引用独立的 [ESP8266 RTOS SDK v3.4](https://github.com/espressif/ESP8266_RTOS_SDK/tree/v3.4)，只包含 StudioX 编写的原生应用模板、器件元数据和上游链接，没有复制完整 SDK。ESP8266 不属于 IDF 5.5.4 的支持目标。

## GigaDevice：GD32

13 个公开包的主要来源如下。包内保留原厂源文件的版权及用途限制、适用的 GigaDevice 软件许可，以及需要的 Arm CMSIS/RISC-V 许可。GigaDevice 的 SLA-GD0001-version1.1 允许在保留许可材料的条件下再分发源代码，并限制其用于 GigaDevice 器件；包中的厂商文件不改授予仓库自身许可。E50x 包含该许可的 PDF 正文。VF103 的部分源文件按自身声明适用 Apache-2.0。

| 子系列 | 公开包版本 | 固定来源 |
| --- | --- | --- |
| GD32C10X | 0.1.0 | [GD32C10X SDK](https://github.com/GigaDevice-GD32-MCU/GD32C10x_Firmware_Library/tree/27bffbe6b94e0250a6dbab8af48f8ca39066131e) |
| GD32E10X | 0.1.0 | [GD32E10X SDK](https://github.com/GigaDevice-GD32-MCU/GD32E10x_Firmware_Library/tree/f5d94ecaa41043fcd56bb4480721d950cc175d3d) |
| GD32E23X | 0.1.0 | [GD32E23X SDK](https://github.com/GigaDevice-GD32-MCU/GD32E23x_Firmware_Library/tree/5b0872e3097fcc3917f5da50ad56d565893771a0) |
| GD32E50X | 0.1.0 | [GD32E50X SDK](https://www.gd32mcu.com/download/down/document_id/282/path_type/1) |
| GD32F10X | 0.1.0 | [GD32F10X SDK](https://github.com/GigaDevice-GD32-MCU/GD32F10x_Firmware_Library/tree/23a80f96368336b4d47014da33cd9b7ba550165e) |
| GD32F1X0 | 0.1.0 | [GD32F1X0 SDK](https://github.com/GigaDevice-GD32-MCU/GD32F1x0_Firmware_Library/tree/5aa55a96aef2420309461466c48723a29f366ed0) |
| GD32F20X | 0.1.0 | [GD32F20X SDK](https://github.com/GigaDevice-GD32-MCU/GD32F20x_Firmware_Library/tree/8af0037e4de77b063716aaf77088f31764fea78d) |
| GD32F30X | 0.1.1 | [GD32F30X SDK](https://github.com/GigaDevice-GD32-MCU/GD32F30x_Firmware_Library/tree/c66ff9a5b43e1a93e1dff0b21d934f10ace90e0a) |
| GD32F3X0 | 0.1.1 | [GD32F3X0 SDK](https://github.com/GigaDevice-GD32-MCU/GD32F3x0_Firmware_Library/tree/bff30ad10ebd2ef41752b25b79360ec9fd634a80) |
| GD32F403 | 0.1.1 | [GD32F403 SDK](https://github.com/GigaDevice-GD32-MCU/GD32F403_Firmware_Library/tree/7278afc660348780832276e6e5c6ddb65e75ad77) |
| GD32F4XX | 0.1.1 | [GD32F4XX SDK](https://github.com/GigaDevice-GD32-MCU/GD32F4xx_Firmware_Library/tree/10d02f4c8a7e1d79da8b2a9ad67b534f187ec936) |
| GD32L23X | 0.1.0 | [GD32L23X SDK](https://github.com/GigaDevice-GD32-MCU/GD32L23x_Firmware_Library/tree/88070a413213265b5e4fc6162f25f754fb912e96) |
| GD32VF103 | 0.1.0 | [GD32VF103 SDK](https://github.com/GigaDevice-GD32-MCU/GD32VF103_Firmware_Library/tree/908b7f3bb4292f5cf1a676fe12667467273a5b31) |

合计收录 398 个容量/封装基础型号，器件表来自包中记录的官方 DFP，原始来源哈希及启动文件转换记录保留。GD32F30x/F3x0/F403/F4xx 的 **0.1.1** 公开修订只补入 Apache-2.0 CMSIS 许可正文，更新版本和索引；原厂 SDK 源文件、器件参数、模板和编译配置未变。

GD32E51x 本次不公开：当前来源包含 SLA-GD0006-version1.1 约束的组件，该许可未提供本仓库需要的再分发授权。它不能套用其他 GD32 包的 SLA-GD0001 条款。

## STC：8 位系列

STC 包中的 SFR 名称和地址来自厂商 AiCube 头文件，采用 StudioX 自己的声明格式重新生成；不复制原头文件注释、示例或原始文件布局。原 AiCube 文件没有已核实的再分发许可，因此不分发原始头文件或 AiCube 二进制。具体来源哈希与生成方式在 `vendor/provenance.json` 记录；型号与容量另外由包中的厂商资料链接核对。

## 本次未公开的本地包

WCH CH32V203、CH32V307、CH592、CH595 的当前 SDK 仅保留厂商版权及仅用于 WCH 芯片的声明，缺少已核实的再分发许可。FreeRTOS 的 MIT 许可只覆盖 FreeRTOS 文件，不能作为 WCH SDK 的授权。AGM 临时包缺少原 SDK 再分发许可。这些本地包没有上传到本仓库。[UPDATE-0.2.5.md](UPDATE-0.2.5.md)列出准确范围。


## 2026-09-30 新增 ARM32 包

固定的 DFP 版本、SDK 提交、URL 和 SHA-256 见 [sources.lock.json](validation/arm32-2026-09-30/sources.lock.json)，补充许可的固定提交和哈希见 [publication-policy.json](validation/arm32-2026-09-30/publication-policy.json)。每包保留原始来源、许可证、逐文件哈希及转换前的启动文件。官方商标只表示目标兼容性，这些包由 StudioX 整理，不表示厂商认可。

| 来源 | 此次公开内容与条款依据 |
| --- | --- |
| STMicroelectronics | 126 个新增子系列包使用 ST 官方 CMSIS Device 仓库；DFP 只提供器件描述数据，CMSIS/启动文件保留其原 Apache-2.0 / BSD 条款及 LICENSE.md。 |
| ArteryTek | 29 包；厂商文件内明确允许为雅特力 MCU 开发而使用、复制、分发 BSP，保留用途条件、版权和免责声明。 |
| Geehy | 18 包；补入相应 F0/F10/F4 官方 SDK 的 Geehy Semiconductor Software License Agreement 1.3 全文。允许按第 4 节保留声明后分发源码及修改版本；限制用于相应极海器件，不重新授权为 Apache/BSD/MIT。转换文件带 StudioX 修改说明和日期。 |
| HDSC | 7 包；保留每个文件中仅面向华大器件的用途限制、允许在该用途下复制整体或部分的条款及完整版权/免责声明。 |
| MindMotion | 5 包；保留 DFP 的 Apache-2.0 许可和原文件版权。 |
| NSING | 11 包；所选文件含允许源码/二进制再分发的条款，保留条件和免责声明。N32G003/N32G430 的不同限制不套用到这 11 包，也不以这些许可覆盖那两个受限包。 |
| Nuvoton | 44 包；保留文件中的 Apache-2.0 声明以及所需完整正文。M0A21/NDA102 暂缺覆盖所选文件的明确条款，未上传。 |
| Nordic Semiconductor | 12 包；保留原文件声明和 DFP 附带的 BSD 许可。本次基础包不包含 SoftDevice 无线固件或完整 BLE 协议栈。 |
| Microchip | SAMD21/SAMD51 两包；保留 DFP 的 Apache-2.0 许可、Arm CMSIS 许可和各文件原始声明。 |
| NXP | 18 包；旧 LPC 包保留源文件内的 BSD/开发工具分发条款及 DFP 原许可。6 个 MCUXpresso 包内保留 Software Content Register：所选器件/驱动文件按其 BSD-3-Clause 声明分发，补入 NXP 官方 licenses/COPYING-BSD-3 全文；不将专有中间件授权推及其它组件。 |

全部新包另保留 Arm CMSIS 6.3.0 所需的 Apache-2.0 正文。生成的复位/向量文件随包保留原始文件，新增日期和转换说明不替代其适用条款。编译验证并不证明拥有 SDK 再分发权，因此本轮特定受限/未明确授权的包没有公开；不将本地 330 包 ZIP 作为 GitHub 下载附件。
