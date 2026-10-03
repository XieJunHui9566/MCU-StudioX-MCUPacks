# Espressif 多版本模板

每个 ESP32 目标按 SDK 版本提供独立 StudioX Pack 格式 1 包。包 ID 保持相同，以便 IDE 新建页按明确 SDK、组件和模板建立选择；不同 SDK 的包同时保留。

| ESP-IDF / 开发环境组件 | 器件包版本 | 上游 |
| --- | --- | --- |
| 5.5.4 | 0.1.1 | [v5.5.4](https://github.com/espressif/esp-idf/tree/v5.5.4) |
| 5.5.5 | 0.2.0 | [v5.5.5](https://github.com/espressif/esp-idf/tree/v5.5.5) |
| 6.0.3 | 0.3.0 | [v6.0.3](https://github.com/espressif/esp-idf/tree/v6.0.3) |
| 6.1.0 | 0.4.0 | [v6.1](https://github.com/espressif/esp-idf/tree/v6.1) |

每个版本均提供 ESP32-WROOM-32、ESP32-P4、ESP32-S3、ESP32-C3、ESP32-C5、ESP32-C6 六个目标，各含官方 Hello World 和 FreeRTOS 运行统计模板，共 24 包、48 个 SDK/目标/模板组合。后三版本新增 18 包、36 个组合。ESP8266 继续使用原来的 RTOS SDK 3.4 / 0.1.0 包。

| 目标 | IDF 5.5.4 | IDF 5.5.5 | IDF 6.0.3 | IDF 6.1.0 |
| --- | --- | --- | --- | --- |
| ESP32-WROOM-32 | [0.1.1](espressif.esp32-wroom-32-0.1.1.mcupack) | [0.2.0](espressif.esp32-wroom-32-0.2.0.mcupack) | [0.3.0](espressif.esp32-wroom-32-0.3.0.mcupack) | [0.4.0](espressif.esp32-wroom-32-0.4.0.mcupack) |
| ESP32-P4 | [0.1.1](espressif.esp32p4-0.1.1.mcupack) | [0.2.0](espressif.esp32p4-0.2.0.mcupack) | [0.3.0](espressif.esp32p4-0.3.0.mcupack) | [0.4.0](espressif.esp32p4-0.4.0.mcupack) |
| ESP32-S3 | [0.1.1](espressif.esp32s3-0.1.1.mcupack) | [0.2.0](espressif.esp32s3-0.2.0.mcupack) | [0.3.0](espressif.esp32s3-0.3.0.mcupack) | [0.4.0](espressif.esp32s3-0.4.0.mcupack) |
| ESP32-C3 | [0.1.1](espressif.esp32c3-0.1.1.mcupack) | [0.2.0](espressif.esp32c3-0.2.0.mcupack) | [0.3.0](espressif.esp32c3-0.3.0.mcupack) | [0.4.0](espressif.esp32c3-0.4.0.mcupack) |
| ESP32-C5 | [0.1.1](espressif.esp32c5-0.1.1.mcupack) | [0.2.0](espressif.esp32c5-0.2.0.mcupack) | [0.3.0](espressif.esp32c5-0.3.0.mcupack) | [0.4.0](espressif.esp32c5-0.4.0.mcupack) |
| ESP32-C6 | [0.1.1](espressif.esp32c6-0.1.1.mcupack) | [0.2.0](espressif.esp32c6-0.2.0.mcupack) | [0.3.0](espressif.esp32c6-0.3.0.mcupack) | [0.4.0](espressif.esp32c6-0.4.0.mcupack) |

文件名为 `espressif.<目标>-<器件包版本>.mcupack`，可直接从本目录下载所需版本，在 IDE 的器件包导入入口导入。随后新建页选择准确目标、模板和 IDF 版本；所需开发环境组件从 [Toolchains](https://github.com/XieJunHui9566/MCU-StudioX-Toolchains) 获取或手动导入。SDK、组件、器件包和 IDE 分别管理版本，安装其他组件不会替换已有工程的锁。

目录中 ESP32 包声明 `retainVersion: true`。支持该字段的 IDE 联网同步会补齐全部明确保留版本；早期只同步最高包版本的 IDE 仍可手动导入所需包。导入和构建继续核对文件哈希、SDK 版本、目标和组件内容锁。

各版本使用对应固定上游提交的原始示例，保留 CC0/公共领域声明及 SDK Apache-2.0 LICENSE。原始与规范化 SHA-256、上游链接和公开组件指纹在 [验证目录](../validation/esp-idf-2026-10-04)。这里只分发小型模板与元数据，完整 SDK、编译器和 Python 不放进 `.mcupack`。
