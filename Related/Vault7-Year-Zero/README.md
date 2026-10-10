# Vault 7 主档案：Year Zero 中文说明

## 资料定位

**Year Zero** 是 WikiLeaks 于 2017 年 3 月公开的 Vault 7 第一部分，主题是 CIA 的网络攻击、恶意软件和远程监控能力。官方页面称首批发布包含约 8,761 份文档和文件，资料时间范围主要覆盖 2013-2016 年。

- 官方主页：[Vault 7 - CIA Hacking Tools Revealed](https://wikileaks.org/ciav7p1/)
- 公开内容：[Year Zero 官方发布页](https://wikileaks.org/ciav7p1/)
- 相关项目：[Vault 7 Projects](https://wikileaks.org/vault7/)
- 本地项目资料：[Vault7 项目中文索引](../../README.md)

## 主要内容

Year Zero 不是单一软件，而是一组来自内部开发协作系统的资料，涉及：

- iPhone、iPad、Android 等移动设备；
- Windows、macOS、Linux、Solaris 等操作系统；
- 路由器、网络设备和 Web 服务；
- Samsung 智能电视等嵌入式设备；
- USB、光盘和其他可移动介质；
- 恶意软件植入、监听端、命令与控制基础设施；
- 漏洞、零日利用、测试、部署和运维文档。

官方页面提到的项目或组件包括 Weeping Angel、Hammer Drill、Brutal Kangaroo、Assassin、Medusa、Fine Dining、Improvise、HIVE 等。这里的项目名称来自 WikiLeaks 的公开说明；具体功能、版本和适用平台应以对应文档为准。

## 资料形态

公开资料主要是：

1. 内部 Wiki 页面及其版本历史；
2. 项目设计文档、用户指南和管理员指南；
3. 测试记录、配置说明和部署流程；
4. 部分附件、文件名清单、代码片段和技术示例。

WikiLeaks 页面称 Year Zero 包含数千个 Wiki 页面和数百个附件。页面版本历史能够反映文档的演变，但并不代表每个条目都是完整的软件发行包。

## 是否包含完整源代码

不能把 Year Zero 理解为完整的 CIA 源代码仓库。WikiLeaks 官方说明称，其发布时避免直接分发可立即使用的“武器化”网络工具；部分压缩包附件只提供文件名列表，其他二进制附件则以十六进制转储或审查后的形式提供。

因此应区分：

| 内容类型 | Year Zero 中的情况 |
|---|---|
| 设计和操作文档 | 大量存在 |
| 配置、命令和代码片段 | 部分存在 |
| 完整源码仓库 | 未完整公开 |
| 可直接运行的完整植入程序 | 官方发布范围内通常未提供 |
| 二进制附件 | 部分被替换、转储或审查 |

## 与本仓库的关系

本仓库当前已归档的是 Vault 7 Projects 页面中可直接下载的项目文档，例如 Grasshopper、Marble、Scribbles、Hive 和 Brutal Kangaroo 等。这些文件是项目说明、用户指南、测试资料或开发辅助资料，并不等同于 Year Zero 主档案的完整副本。

本仓库还包含：[WikiLeaks 十周年资料包](../WikiLeaks-10years/README.md)。该资料是历史回顾和发布会材料，不是 Year Zero 的技术档案。

## 安全阅读建议

- 仅做静态阅读和文件清单分析。
- 不要直接运行 PDF、ZIP 或其他附件中发现的程序、脚本和宏。
- 不要在日常电脑、生产网络或带有真实凭据的环境中测试。
- 如需研究二进制或脚本，应使用离线虚拟机、快照和无敏感数据的隔离环境。
- 对 WikiLeaks 页面中的数量、功能和归因性陈述，建议与厂商公告、漏洞数据库和独立研究交叉核对。

## 参考

- [Vault 7 官方主页](https://wikileaks.org/ciav7p1/)
- [Vault 7 Projects 项目列表](https://wikileaks.org/vault7/)
- [WikiLeaks 十周年资料](https://wikileaks.org/10years/)
