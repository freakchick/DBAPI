
# DBAPI

**SQL 即 API — 数仓开发者的低代码数据服务利器**

只需编写 SQL，自动生成 HTTP API

<p>
  <a href="https://www.51dbapi.com"><strong>🎬 官网</strong></a>
  <a href="https://www.51dbapi.com/guide"><strong>📖 文档</strong></a> ·
  <a href="https://www.51dbapi.com/demo"><strong>🚀 在线体验</strong></a> ·
  <a href="https://www.51dbapi.com/install"><strong>📥 下载安装</strong></a> ·
</p>

<p>
  <a href="https://gitee.com/freakchicken/db-api">
    <img src="https://img.shields.io/badge/Gitee-db--api-C71D23?logo=gitee" alt="Gitee">
  </a>
  <img src="https://img.shields.io/badge/个人版-v4.0.32-blue" alt="个人版">
  <img src="https://img.shields.io/badge/企业版-v4.6.0-important" alt="企业版">
  <img src="https://img.shields.io/badge/JDK-8%2F11%2F17-brightgreen" alt="JDK">
  <img src="https://img.shields.io/badge/license-个人版免费-ff69b4" alt="License">
</p>

</div>

---

## 什么是 DBAPI？

DBAPI 是一个面向**数据仓库开发人员**的低代码数据服务平台。**在页面上编写 SQL 并配置参数，即可自动生成生产级 HTTP API 接口**，彻底告别重复的 CRUD 代码编写。

- **🎯 定位**：企业数据服务管理中心 — 统一管理、发布、监控、治理所有数据接口
- **💡 场景**：BI 报表、数据大屏、前端快速原型、AI 应用数据接入
- **⚡ 理念**：SQL 即接口，极致效率

---

## 核心特性

### 🚀 开箱即用，轻量部署

- 无需编程，不依赖其他软件（仅需 Java 运行环境）
- 2 核 4G 服务器即可稳定运行
- 支持单机 / 集群模式，支持 Windows / Linux

### 🔌 数据源广泛兼容

| 类型 | 支持 |
|------|------|
| **关系型数据库** | MySQL、SQL Server、PostgreSQL、Oracle、Hive、达梦、人大金仓、Doris、OceanBase、GaussDB 等**所有** JDBC 协议数据库 |
| **Elasticsearch** | ES DSL 执行器，直接执行 Elasticsearch 查询 |
| **HTTP 代理** | HTTP 执行器，转发第三方 REST 接口 |

### ✍️ 动态 SQL，MyBatis 风格

- 支持 `#{}` / `${}` 参数绑定，完整 MyBatis 动态 SQL 语法
- SQL 编辑器内置**运行 / 调试**功能，所见即所得
- 支持 Select / Insert / Update / Delete 及存储过程
- 多 SQL 组合执行，灵活控制事务开关

### 🔄 API 编排

- **DAG 可视化画布**：拖拽式编排，无需写代码
- 支持开始 → API 执行 → 判断（If/Else）→ 结束节点
- 前序 API 结果直接作为后续步骤输入
- Groovy 脚本计算，灵活处理数据

### 🛡️ 企业级安全防护

| 能力 | 说明 |
|------|------|
| **动态鉴权** | clientId + secret 获取 Token，API 级别访问控制 |
| **IP 防火墙** | IP 白名单 / 黑名单拦截 |
| **精准限流** | API 级 QPS 限流 |
| **数据加密** | 响应数据 RSA 加密，请求参数数字签名 |
| **审计日志** | 全量操作审计 |

### 🧩 插件体系（5 大类）

- **缓存插件** — Redis / Ehcache / ES 等
- **数据转换插件** — 数据脱敏、格式重组
- **告警插件** — 邮件、短信、钉钉、飞书、企业微信
- **参数处理插件** — 参数解密、校验、转换
- **全局数据转换插件** — 适配 AMIS 等前端框架

### 🤖 AI + MCP 支持

- 将 DBAPI 的数据 API 映射为 **MCP 工具**
- 对接 Claude Desktop、Cursor、LangChain、Spring AI 等 AI 客户端
- 支持AI助手，自然语言生成SQL

### 📊 监控与日志

- API 调用记录查询 & 访问统计
- 日志落库：ClickHouse / MySQL / PostgreSQL / Doris
- 支持 Kafka 缓冲采集，适合大规模场景

### 🛠️ 更多能力

- API 动态创建 / 修改 / 下线，**热部署无感知**
- API 分组管理、导入导出、版本回滚（企业版）
- API 内置变量 `__clientId`、`__apiId`
- OpenAPI 接口，便于系统集成
- 数据源健康检查，请求测试参数预设

---

## 快速开始

### 1. 环境要求

- JDK 8 / 11 / 17
- OpenSSL 3（Windows 无需）

### 2. 下载 & 启动

```bash
# 下载个人版（免费）
wget https://img.51dbapi.com/dbapi/dbapi-4.0.32-bin.tar.gz
tar -xzf dbapi-4.0.32-bin.tar.gz
cd dbapi-4.0.32

# 修改数据库配置（默认使用内嵌 SQLite）
# vim conf/application.properties

# 启动服务
bash bin/dbapi-daemon.sh start standalone
```

### 3. 访问系统

浏览器打开 `http://<your-ip>:8520`，默认账号密码 `admin / admin`。

> 详细安装文档请参考 [📖 安装指南](https://www.51dbapi.com/install)

---


## 在线体验

- **演示环境**：[https://www.51dbapi.com/demo](https://www.51dbapi.com/demo)（账号/密码：`admin / admin`）

---

## 社区

- **Gitee**：[https://gitee.com/freakchicken/db-api](https://gitee.com/freakchicken/db-api)
- **官网**：[https://www.51dbapi.com/guide](https://www.51dbapi.com/guide)
- **文档**：[https://www.51dbapi.com](https://www.51dbapi.com)

---

*如果 DBAPI 对你有帮助，欢迎在 Gitee 给项目点个 ⭐*
