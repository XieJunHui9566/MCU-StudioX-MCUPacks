# 第三方来源与许可

本仓库是器件包的分发目录，不对包内所有源码统一授予一种开源许可。使用或再分发某个包时，应遵守该包中原有的版权声明和许可。以下列出当前 40 个包的主要来源；逐文件来源及哈希见包内 `provenance.json`。

## Puya：PY32F0、PY32F403、PY32F410、PY32F420

16 个包采用 [OpenPuya 社区镜像](https://github.com/OpenPuya)中的固件源码。OpenPuya 不是普冉官方代码仓库。型号、封装和容量另外按普冉产品资料核对；这些包不代表普冉官方发布或认可。每个包的 `provenance.json` 记录具体镜像、提交和源文件哈希。

PY32F0 包内保留 `licenses/Puya-BSD-3-Clause.txt`；含 Apache-2.0 CMSIS 文件的 9 个修订包还保留 `licenses/CMSIS-LICENSE.txt`。F002A/F002B/F003/F030 的 Arm CMSIS 文件使用源文件中完整保留的 BSD 许可声明，无需另附 Apache 许可。PY32F403/F410/F420 包内保留 `licenses/OpenPuya-BSD-3-Clause.txt` 与 `licenses/CMSIS-LICENSE.txt`（Apache-2.0）。Puya、STMicroelectronics、OpenPuya 和 Arm 源文件中的原版权声明均保留。具体文件适用其自身声明的许可；请勿把仓库说明或其他项目的许可覆盖到这些第三方文件。

## Raspberry Pi：RP2350

该包的 SDK 来源是 [Raspberry Pi Pico SDK 2.2.0](https://github.com/raspberrypi/pico-sdk/tree/2.2.0)。包内 `sdk/LICENSE.TXT` 保留 SDK 的 BSD-3-Clause 许可。`sdk/src/rp2_common/pico_printf/` 下的第三方 printf 源文件另在文件头保留完整 MIT 许可和作者声明。

## STMicroelectronics：STM32F1、STM32F4

23 个 0.1.2 包的 CMSIS/CMSIS Device、HAL 与启动文件分别来自 ST 官方 [STM32CubeF1 v1.8.7](https://github.com/STMicroelectronics/STM32CubeF1/tree/v1.8.7) 和 [STM32CubeF4 v1.28.3](https://github.com/STMicroelectronics/STM32CubeF4/tree/v1.28.3)；FreeRTOS 10.3.1 来自后者。包内 `licenses/` 保留 CMSIS/CMSIS Device 的 Apache-2.0、ST HAL 的 BSD-3-Clause、FreeRTOS 的 MIT 许可及 STM32Cube 软件清单，源码原版权声明未改。`provenance.json` 列有收入包中的每个 SDK 文件 SHA-256。包内没有 SPL 或 Keil DFP 的器件头文件，也没有工具链二进制；请勿把仓库自身许可证套用到这些第三方组件。

这些第三方商标只用于说明器件兼容性，不表示相应厂商为本仓库背书。
