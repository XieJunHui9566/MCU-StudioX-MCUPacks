# 第三方来源与许可

本仓库是器件包的分发目录，不对包内所有源码统一授予一种开源许可。使用或再分发某个包时，应遵守该包中原有的版权声明和许可。以下仅列出当前四个包的主要来源；逐文件来源及哈希见包内 `provenance.json`。

## Puya：PY32F403、PY32F410、PY32F420

三个包采用 [OpenPuya 社区镜像](https://github.com/OpenPuya/PY32F4xx_Firmware)中的固件源码。OpenPuya 不是普冉官方代码仓库。型号、封装和容量另外按普冉产品资料核对；这些包不代表普冉官方发布或认可。

包内保留 `licenses/OpenPuya-BSD-3-Clause.txt` 与 `licenses/CMSIS-LICENSE.txt`（Apache-2.0），以及 Puya、STMicroelectronics 和 Arm 源文件中的原版权声明。具体文件适用其自身声明的许可；请勿把仓库说明或其他项目的许可覆盖到这些第三方文件。

## Raspberry Pi：RP2350

该包的 SDK 来源是 [Raspberry Pi Pico SDK 2.2.0](https://github.com/raspberrypi/pico-sdk/tree/2.2.0)。包内 `sdk/LICENSE.TXT` 保留 SDK 的 BSD-3-Clause 许可。`sdk/src/rp2_common/pico_printf/` 下的第三方 printf 源文件另在文件头保留完整 MIT 许可和作者声明。

这些第三方商标只用于说明器件兼容性，不表示相应厂商为本仓库背书。
