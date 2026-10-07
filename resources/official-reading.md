# 按实际问题查找官方资料

这里收录官方文档入口，并附原创的阅读建议与练习。没有复制文章正文、配图或视频；链接页面及其中的示例适用各自的版权与许可条款。

## 部署与恢复

| 你遇到的问题 | 官方入口 | 可以做的小练习 |
| --- | --- | --- |
| 同一份程序怎样在不同环境运行 | [Spring Boot 外部化配置](https://docs.spring.io/spring-boot/reference/features/external-config.html) | 给测试环境增加一个无秘密的配置项，确认配置来源和覆盖次序 |
| 容器更新后如何保留文件 | [Docker Volumes](https://docs.docker.com/engine/storage/volumes/) | 用测试卷保存文件，重建测试容器后核对内容 |
| 上传分片为什么被代理拒绝 | [Nginx client_max_body_size](https://nginx.org/en/docs/http/ngx_http_core_module.html#client_max_body_size) | 对比合法分片与超限请求的状态码和页面反馈 |
| 数据库备份怎样恢复 | [MySQL 备份与恢复](https://dev.mysql.com/doc/refman/8.4/en/backup-and-recovery.html) | 在隔离实例恢复一份测试备份，核对记录与权限 |

## 浏览器与前端

| 你遇到的问题 | 官方入口 | 可以做的小练习 |
| --- | --- | --- |
| 大文件下载怎样继续读取 | [MDN HTTP Range Requests](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Range_requests) | 检查测试文件的 206、Content-Range 和无效范围响应 |
| Vue 表单状态怎样组织 | [Vue 官方指南](https://vuejs.org/guide/introduction.html) | 把加载、空态、失败和成功做成明确可切换的状态 |
| 怎么在不同引擎跑同一流程 | [Playwright 浏览器说明](https://playwright.dev/docs/browsers) | 跑同一份无真实用户数据的下载用例，记录引擎与版本 |
| 动画怎样尊重用户偏好 | [MDN prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion) | 开启系统减少动画选项，验证页面内容仍完整可用 |

## AI 与服务端边界

| 你遇到的问题 | 官方入口 | 可以做的小练习 |
| --- | --- | --- |
| DeepSeek 接口需要哪些参数 | [DeepSeek API 文档](https://api-docs.deepseek.com/) | 用虚构内容验证模型、输出预算与错误提示，记录实际费用 |
| 自定义模型地址可能访问哪里 | [OWASP SSRF Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Server_Side_Request_Forgery_Prevention_Cheat_Sheet.html) | 用本地夹具验证地址、DNS 和重定向限制 |
| AI Key 应如何保存和轮换 | [OWASP Secrets Management Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html) | 画出密钥从录入、加密、调用到删除的生命周期 |
| 日志如何帮助排错又不泄漏内容 | [OWASP Logging Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Logging_Cheat_Sheet.html) | 让测试请求失败，核对日志不含密钥、正文和附件内容 |

阅读时先确认文档版本与项目使用版本一致。涉及转载代码片段时，应另外核对该片段的许可与署名要求；“能够访问”不等于“可随意转载”。

[返回笔记首页](../README.md)
