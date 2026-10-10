# Vault 7 Projects：中文索引与项目介绍

> 来源： [WikiLeaks Vault 7: Projects](https://wikileaks.org/vault7/)。本文根据项目主页的公开说明、项目页面标题及本地归档文件整理；“技术主题”中的概括性表述是对网页内容的中文归纳，不代表对文件真实性或当前适用性的独立鉴定。
>
> 本地归档：86 份文件，按项目分类保存于本目录；文件校验值见 [`manifest.csv`](./manifest.csv)。文档多为历史资料，阅读、解压和分析时建议使用隔离环境，不要直接运行未知程序或宏。

## 项目索引

| 项目 | WikiLeaks 发布时间 | 本地目录 |
|---|---:|---|
| [Protego](#1-protego) | 2017-09-07 | [Protego](./Protego/) |
| [Angelfire](#2-angelfire) | 2017-08-31 | [Angelfire](./Angelfire/) |
| [ExpressLane](#3-expresslane) | 2017-08-24 | [ExpressLane](./ExpressLane/) |
| [CouchPotato](#4-couchpotato) | 2017-08-10 | [CouchPotato](./CouchPotato/) |
| [Dumbo](#5-dumbo) | 2017-08-03 | [Dumbo](./Dumbo/) |
| [Imperial / UCL / Raytheon](#6-imperial--ucl--raytheon) | 2017-07-27 | [UCL-Raytheon](./UCL-Raytheon/) |
| [HighRise](#7-highrise) | 2017-07-13 | [Highrise](./Highrise/) |
| [BothanSpy](#8-bothanspy) | 2017-07-06 | [BothanSpy](./BothanSpy/) |
| [OutlawCountry](#9-outlawcountry) | 2017-06-30 | [OutlawCountry](./OutlawCountry/) |
| [Elsa](#10-elsa) | 2017-06-28 | [Elsa](./Elsa/) |
| [Brutal Kangaroo](#11-brutal-kangaroo) | 2017-06-22 | [Brutal-Kangaroo](./Brutal-Kangaroo/) |
| [Cherry Blossom](#12-cherry-blossom) | 2017-06-15 | [Cherry-Blossom](./Cherry-Blossom/) |
| [Pandemic](#13-pandemic) | 2017-06-01 | [Pandemic](./Pandemic/) |
| [Athena](#14-athena) | 2017-05-19 | [Athena](./Athena/) |
| [AfterMidnight](#15-aftermidnight) | 2017-05-12 | [AfterMidnight](./AfterMidnight/) |
| [Archimedes](#16-archimedes) | 2017-05-05 | [Archimedes](./Archimedes/) |
| [Scribbles](#17-scribbles) | 2017-04-28 | [Scribbles](./Scribbles/) |
| [Weeping Angel](#18-weeping-angel) | 2017-04-21 | 归档于 [Other](./Other/) |
| [Hive](#19-hive) | 2017-04-14 | [Hive](./Hive/) |
| [Grasshopper](#20-grasshopper) | 2017-04-07 | [Grasshopper](./Grasshopper/) |
| [Marble Framework](#21-marble-framework) | 2017-03-31 | [Marble](./Marble/) |
| [Dark Matter](#22-dark-matter) | 2017-03-23 | [DarkMatter](./DarkMatter/) |

## 项目介绍

### 1. Protego

Protego 是 Vault 7 Projects 系列中较为特殊的一组资料。主页将它描述为与 PIC 微控制器相关的导弹控制系统项目，而不是通常意义上的终端恶意软件项目。资料涉及机载主处理器、部署盒、导弹/发射管/接口处的智能开关，以及组件之间的加密认证通信。

其设计重点是授权条件和失效保护：系统需要同时获得边界、有效 GPS 和运行时间窗口等信号，才允许进入规定操作状态；在离开区域、超过时间或发生异常时，还涉及密钥销毁等保护逻辑。本地目录包含系统硬件说明、构建流程、消息格式和软件变更请求资料，适合从嵌入式系统架构、协议设计和安全控制角度阅读。

### 2. Angelfire

Angelfire 是面向 Windows XP/Windows 7 的持久化植入框架。主页将其拆分为 Solartime、Wolfcreek、Keystone、BadMFS 和 Windows Transitory File System 等组件，核心思路是让启动过程加载框架，再由框架装载其他植入模块。

资料特别强调隐蔽存储和减少磁盘痕迹：BadMFS 被描述为用于保存驱动和植入模块的加密/混淆文件系统，Keystone 负责启动用户态应用，瞬态文件机制则用于安装、添加和移除组件。本地目录中的用户指南、开发指南、测试矩阵和笔记可用于研究启动链、模块化设计、内存泄漏风险及取证痕迹。

### 3. ExpressLane

ExpressLane 主页描述的是针对联络机构所部署生物识别系统的数据获取工具。网页叙述的场景是：相关系统由 OTS 提供给合作或联络机构，操作人员以升级生物识别软件为掩护，在现场维护过程中收集数据。

其值得关注的主题包括社会工程式维护场景、升级界面伪装、数据暂存与外带，以及供应方与使用方之间的信任关系。本地文件包括 Tool Delivery Review、TPP、用户手册和需求说明，建议将它们作为需求、交付流程和威胁建模材料交叉阅读，而不要只按单一“恶意软件”视角理解。

### 4. CouchPotato

CouchPotato 的本地归档以用户指南为主。根据项目名称和页面分类，它属于 Vault 7 中面向目标系统的数据获取/监控工具资料。公开页面提供的内容较短，因此对其具体实现不宜超出文档本身作过度推断。

阅读时可重点记录：支持的目标平台、部署前置条件、配置项、采集对象、输出格式、清理机制以及与其他框架的依赖。相关文件见 [CouchPotato](./CouchPotato/)。

### 5. Dumbo

Dumbo 的归档包含多个版本的 Field Guide、User Guide 和早期 TDR/简报资料，体现出一个经过版本演进、并具有现场操作流程的项目。文件组合比单一用户手册更适合用于比较版本差异和功能成熟度。

建议优先阅读 Field Guide 了解使用边界，再对照 User Guide 和 TDR 记录需求、部署流程、设备兼容性和测试证据。这里的介绍仅按 WikiLeaks 页面及文件标题归纳，具体功能以各版本文档为准。

### 6. Imperial / UCL / Raytheon

主页将该发布日期下的内容标为 Imperial，并同时展示 UCL / Raytheon 相关材料。本地归档包括 Achilles、SeaPea、Aeris，以及若干 HTTPBrowser、NfLog、Symantec、FireEye 和 VB/Gamker 相关文档，说明这一组更像若干研究、工具或外部材料的集合，而非单一组件。

阅读时应按文档标题分别建立证据链，区分项目内部设计资料、外部厂商/研究资料和威胁样本分析，避免把同一发布日期下的所有文件误认为一个统一产品。

### 7. HighRise

HighRise 的本地资料主要是 2.0 用户指南。项目页面信息相对简短，因此更适合通过用户指南确认其平台、配置、操作流程和限制条件，再与其他 Vault 7 项目进行横向比较。

建议记录文档中的版本号、运行权限、输入输出、日志位置和卸载/清理步骤；这些字段对历史软件的取证和复现研究比项目宣传性描述更有价值。

### 8. BothanSpy

BothanSpy 的归档包含 1.0 版本的 S-NF 文档，并与 Gyrfalcon 用户手册一同归入该项目组。资料重点可理解为 Windows 凭据/会话相关的工具链和配套说明，但具体采集对象、版本范围和部署方式应以文档正文为准。

阅读时建议优先关注凭据在内存、文件和网络边界上的生命周期，以及文档中出现的权限要求、持久化方式和清理动作；不要在真实账户或生产主机上验证。

### 9. OutlawCountry

OutlawCountry 的本地归档包括用户手册和测试计划。项目名称和材料组织方式表明它更偏向网络设备/路由器环境中的工具或植入能力，而测试计划能够帮助区分“设计目标”和“实际验证过的行为”。

建议先读测试计划，提取支持的设备、固件、网络条件和失败模式，再用用户手册核对操作流程。对历史网络设备资料尤其要注意型号、固件和编译环境差异。

### 10. Elsa

Elsa 归档以用户手册为主，属于针对 Windows 环境的监控/数据获取类项目资料。主页提供的概述有限，因此本文不对其具体采集能力作超出文档的断言。

建议从目标平台、输入数据、采集触发条件、保存位置、网络传输和日志痕迹六个方面整理阅读笔记，并将所有结论标注为“文档明确说明”或“根据配置推断”。

### 11. Brutal Kangaroo

Brutal Kangaroo 目录包含 DriftingDeadline、EzCheese 多个版本的用户指南，以及 IVV/TDR 幻灯片，资料覆盖用户操作、版本差异和验证/评审材料。项目页面将它列为一套较完整的 Windows 工具链资料。

建议按“需求/设计—部署—验证—版本差异”的顺序阅读，重点比较 EzCheese 6.2 与 6.3 的变化，并将幻灯片中的结论回溯到用户指南中的具体章节。

### 12. Cherry Blossom

Cherry Blossom 的归档包括系统需求、快速入门、安装指南、运行环境和 Wi-Fi 设备相关资料，呈现出较完整的部署文档体系。与只包含单份用户手册的项目相比，它更适合分析系统依赖、硬件环境和安装过程。

阅读时应把 Wi-Fi 设备、运行环境和安装步骤放在同一张依赖图中，记录哪些条件是必要条件、哪些只是示例配置，并留意文档中的旧型号和过期软件版本。

### 13. Pandemic

Pandemic 目录包含 1.0/1.1 版本的 S-NF 文档、IVV/RR 检查清单以及版本资料。它的文档组合适合做历史版本比较和测试覆盖分析。

建议先整理版本时间线，再将检查清单中的验证项映射到用户/设计文档；若某项只有检查标题而没有结果，不应将其解读为已通过测试。

### 14. Athena

Athena 的资料包括 Technology Overview、Design、Demo 和 User Guide，说明其既有总体架构描述，也有设计、演示和使用层面的材料。项目主页将其列入面向 Windows 目标环境的 Vault 7 项目系列。

建议按“技术总览—设计—演示—用户指南”顺序阅读，分别提取组件边界、通信方式、部署条件、操作入口和演示中实际展示的能力，避免把 Demo 中的行为泛化为完整产品能力。

### 15. AfterMidnight

AfterMidnight 资料包括用户指南、AlphaGremlin、Assassin 以及图表/图示文件，显示它是由多个组件或配套工具组成的框架。主页将其与 Angelfire、Grasshopper 等持久化框架并列介绍。

图示文件适合先用来建立组件关系，再回到用户指南核对安装、配置、任务调度和清理流程。AlphaGremlin、Assassin 应分别作为子组件阅读，不宜在没有正文证据时合并其功能结论。

### 16. Archimedes

Archimedes 归档包含 1.0 用户指南、1.1/1.2/1.3 Addendum，以及 Fulcrum 用户手册，明显具有持续迭代和补充修订的特点。

建议首先以 1.0 用户指南建立基线，然后按版本顺序阅读 Addendum，制作“新增、删除、修正、未变更”表格；Fulcrum 则单独记录其与 Archimedes 的接口或协作关系。

### 17. Scribbles

Scribbles 目录包括用户指南、IVV/RR 检查清单、Readiness Review Worksheet、EXTENDING 用户指南及配套资料。它提供了从使用到验证、再到扩展的多层文档。

对该项目最有价值的阅读方式是把“功能描述”和“验证证据”分开：用户指南说明目标行为，检查清单和评审工作表说明应如何确认行为，不能仅凭前者判断后者已经完成。

### 18. Weeping Angel

WikiLeaks 将 Weeping Angel 作为独立发布日期项目列出。本地下载目录中未形成同名文件夹，说明该项目页面的实际可下载文件可能被站点组织到其他页面或未被主列表直接提供。

因此，本索引只保留网页项目条目，不虚构具体组件和能力；如需补全，应继续检查该项目专页及其分页链接，并将新增文件单独加入清单。

### 19. Hive

Hive 的本地资料包括用户指南、开发者指南、图表、运行环境和基础设施配置指南，是本批归档中架构/运维资料较完整的项目之一。文件组合表明它不只是单一工具，而是包含服务部署、开发接口和基础设施配置的系统。

建议先读 Operating Environment 和 Infrastructure Configuration，再读 Users/Developers Guide，最后用 figures 对照组件关系。这样可以把运行时依赖、开发接口和操作流程区分开来。

### 20. Grasshopper

Grasshopper 归档包括 1.1 管理员指南、2.0.2 用户指南，以及 StolenGoods 和多个 GH-Module 文档。项目具有框架化和模块化特征，管理员、用户和模块资料分别对应不同的职责边界。

建议按版本和角色分层阅读：先确定 1.1 与 2.0.2 的差异，再单独整理 StolenGoods、Buffalo、Bamboo 和 Null 模块的输入输出、依赖及部署位置。

### 21. Marble Framework

Marble Framework 资料包括 Marble ZIP 归档、Sonic Screwdriver、DerStarke、DarkSeaSkies、FDOS/FIPS 等相关文件。网页对 Marble 的定位是一个用于改变或隐藏文件内容的框架，强调可逆的混淆/处理能力及其对分析工具的影响。

由于该目录含 ZIP 压缩包和多个配套项目，建议先只做静态解包和文件清单分析，记录压缩包内目录、脚本、配置和文档，不直接运行其中的程序。各子项目应分别标注为框架组件、部署工具或测试/环境资料。

### 22. Dark Matter

Dark Matter 是 Vault 7 Projects 列表中最早发布的一组项目资料，归档包含 DerStarke、DarkSeaSkies、FDOS/FIPS 等文档。其资料组合反映出对固件、磁盘/启动环境或底层系统组件的关注，但具体能力必须以各份文档的正文和版本为准。

建议从运行环境和测试计划入手，再阅读用户/设计资料；对于涉及启动链、文件系统或固件的内容，应在离线虚拟机或专用分析环境中进行，不要在日常电脑上尝试部署。

## 建议的阅读顺序

1. 先读本页索引和 `manifest.csv`，确认文件范围与校验值。
2. 先看有完整文档体系的项目：Hive、Cherry Blossom、Scribbles、Brutal Kangaroo、Grasshopper。
3. 再做版本比较：Dumbo、Pandemic、Archimedes、EzCheese。
4. 最后阅读涉及启动链、固件、网络设备或底层环境的资料：Angelfire、Marble、Dark Matter、OutlawCountry。
5. 对所有 PDF 只做静态阅读；任何可执行文件、脚本、宏或压缩包内容均应在隔离环境中处理。

## 归档说明

- 下载范围：Vault 7 Projects 主列表可解析到的全部项目文档链接。
- 本地文件：86 份，合计约 50.95 MB。
- 完整性：所有清单条目均存在，SHA-256 复核无不匹配。
- 下载脚本：[download-vault7.ps1](./download-vault7.ps1)。
- 原始来源：[WikiLeaks Vault 7: Projects](https://wikileaks.org/vault7/)。
