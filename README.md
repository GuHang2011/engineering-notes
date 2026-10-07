# Engineering Field Notes | 工程实践笔记

高校资料协作系统、AI 办公工具和数据项目中的实践复盘，重点记录设计取舍、验证边界和部署注意事项。

这些内容根据个人项目经验重新整理，公开设计思路、验证记录与检查模板。项目完整源码和实际业务数据不在本仓库发布。

第一次阅读可以从[上线检查表](templates/release-checklist.md)开始；评估“500 人在线”时，先看[容量测试复盘](notes/capacity-testing.md)与[报告模板](templates/capacity-report.md)。

## 笔记

| 主题 | 内容 |
| --- | --- |
| [学校内网系统部署](notes/campus-system-deployment.md) | 容器边界、配置、持久化、备份与上线检查 |
| [容量测试该如何解读](notes/capacity-testing.md) | 会话数、请求负载、数据库、文件传输和测试范围 |
| [个人 AI 密钥与模型接入](notes/personal-ai-keys.md) | BYOK、密钥保存、模型端点和人工确认 |
| [大文件分片传输](notes/large-file-transfer.md) | 分片、幂等、权限、磁盘和浏览器下载行为 |
| [浏览器兼容实践](notes/browser-compatibility.md) | 文件下载、存储降级、日期和移动端验证 |
| [AI 办公中的人工把关](notes/human-reviewed-ai-workflows.md) | 草稿生成、PPT 导出和可追溯的操作边界 |

## 可复用模板

| 模板 | 使用时机 |
| --- | --- |
| [发布与恢复检查表](templates/release-checklist.md) | 部署前、升级前和恢复演练时填写 |
| [容量测试报告](templates/capacity-report.md) | 把环境、负载、结果、异常和结论边界写在同一份报告里 |
| [个人 AI 接入验收表](templates/ai-provider-checklist.md) | 新增模型服务商或修改密钥、调用和导出流程时核对 |

模板中的空白字段需要按实际项目填写，勾选项需要有对应证据。

## 官方资料导航

[按问题查找官方文档](resources/official-reading.md)：部署与备份、浏览器文件行为、AI 接口和服务端安全。每个入口都附有适合解决的问题和阅读后可以尝试的小练习。

## 范围

容量和浏览器测试记录来自个人开发环境中的项目验证，只能说明对应环境、数据和测试脚本的结果。它们不是学校生产环境的性能承诺，也不替代安全审计、真机验收或恢复演练。上线前应根据实际服务器、网络、数据规模和学校流程重新验证。

部分笔记链接到官方技术文档，作为进一步阅读入口。所有说明均为概述和经验整理，不构成对第三方产品的背书。

## 内容来源与使用

六篇笔记依据本地高校资料归档与协作项目的部署、容量、AI、聊天和浏览器验证记录整理。文中已发生的测试与建议后续执行的检查分别表述，容量数据对应 2026-10-06 的开发环境记录。

文章、模板与导航说明为本次原创整理；没有转载第三方文章、图片或视频。外链资料版权归其权利人，阅读入口不代表获得再分发许可。仓库目前未授予通用再许可；需要再分发或改编时，请通过 [Issue](https://github.com/GuHang2011/engineering-notes/issues) 联系作者确认范围。报告模板请勿填写真实口令或学生、教师个人资料。

## 关于作者

- GitHub: [@GuHang2011](https://github.com/GuHang2011)
- Academic portfolio: [guhang2011.github.io](https://guhang2011.github.io/)
- Profile: [README](https://github.com/GuHang2011/GuHang2011)
