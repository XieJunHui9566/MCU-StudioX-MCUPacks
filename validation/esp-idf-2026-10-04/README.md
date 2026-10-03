# ESP-IDF 多版本模板验证

这次新增 IDF 5.5.5、6.0.3、6.1.0 三组独立器件包，分别为 0.2.0、0.3.0、0.4.0。各组覆盖 ESP32-WROOM-32、C3、C5、C6、P4、S3，每目标提供 Hello World 和 FreeRTOS 运行统计，共 18 包、36 个新增组合。原 5.5.4 / 0.1.1 包继续保留。

## 固定来源

| SDK | 官方标签 | 上游提交 | 模板记录 |
| --- | --- | --- | --- |
| 5.5.5 | [v5.5.5](https://github.com/espressif/esp-idf/releases/tag/v5.5.5) | b774170ff46c393eeb5e495ea37936038d3f4f4f | [来源与 SHA-256](template-sources-5.5.5.json) |
| 6.0.3 | [v6.0.3](https://github.com/espressif/esp-idf/releases/tag/v6.0.3) | 76f5dedd9950a3012fee8fb7d5586df21fc67802 | [来源与 SHA-256](template-sources-6.0.3.json) |
| 6.1.0 | [v6.1](https://github.com/espressif/esp-idf/releases/tag/v6.1) | fff9895c82d744c7237be8847347bdd1b07c6643 | [来源与 SHA-256](template-sources-6.1.0.json) |

原始源码来自上述不可变提交，仅将 CRLF 规范化为 LF。逐文件原始和规范化摘要、目标支持文件、许可证和公开开发环境组件清单指纹均保留；包不包含完整 SDK 或工具链。

## 验证范围

三组 SDK 各自完成六目标 × 两模板的 12/12 原生编译，总计 **36/36 通过**。四版本包的导入、48 个工程生成与真实目录同步共 **441 项检查通过**；IDE Release 全量构建为 0 警告、0 错误。

[result.json](result.json) 保存最终汇总，包含 36 个新增 SDK/目标/模板组合的真实原生 SDK 构建结果、固件大小与 SHA-256，组件身份及模板输入摘要。此处记录的是离线软件验证，没有连接、下载或调试实板。

维护入口在 IDE 仓库的 `tools/StudioX.EspressifPackSetValidation`。`inspect` 模式使用真实待发布目录验证 24 个四版本 ESP32 包、48 个模板工程、版本选择、并存可见性、增量同步与重复同步。指定 SDK 则通过 Engine/BuildService 和已有精确组件编译六目标的两模板。`StudioX.RemotePackValidation` 另外覆盖没有 retainVersion 字段的旧目录、普通包最高版本更新、坏哈希、越界路径及保留版本补齐。

原始构建日志、工程、组件全量校验和固件留在本地隔离验证目录；公开记录不含机器路径、硬件备份或账户信息。原有 334 包的文件、大小和 SHA-256 在目录更新前后均核对。现有工程不会因新增模板或安装其它 SDK 改变。
