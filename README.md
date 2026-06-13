# DBAPI

[![EN doc](https://img.shields.io/badge/document-English-blue.svg)](README.md)
[![CN doc](https://img.shields.io/badge/文档-中文版-blue.svg)](README_zh_CN.md)

**SQL is API — Low-code data service tool for data warehouse developers**

Just write SQL, auto-generate HTTP APIs

<p>
  <a href="https://www.51dbapi.com/en"><strong>🎬 Website</strong></a>
  <a href="https://www.51dbapi.com/en"><strong>📖 Docs</strong></a> ·
  <a href="https://www.51dbapi.com/demo"><strong>🚀 Live Demo</strong></a> ·
  <a href="https://www.51dbapi.com/en/download"><strong>📥 Download</strong></a> ·
</p>

<p>
  <a href="https://github.com/freakchick/DBApi">
    <img src="https://img.shields.io/badge/GitHub-DBApi-181717?logo=github" alt="GitHub">
  </a>
  <img src="https://img.shields.io/badge/Community-v4.0.32-blue" alt="Community">
  <img src="https://img.shields.io/badge/Enterprise-v4.6.0-important" alt="Enterprise">
  <img src="https://img.shields.io/badge/JDK-8%2F11%2F17-brightgreen" alt="JDK">
  <img src="https://img.shields.io/badge/license-Community%20Free-ff69b4" alt="License">
</p>

---

## What is DBAPI?

DBAPI is a low-code data service platform for **data warehouse developers**. **Write SQL and configure parameters on the page, and it automatically generates production-grade HTTP API endpoints** —告别 repetitive CRUD coding forever.

- **🎯 Positioning**: Enterprise data service management center — centrally manage, publish, monitor, and govern all data APIs
- **💡 Scenarios**: BI reports, data dashboards, rapid frontend prototyping, AI application data integration
- **⚡ Philosophy**: SQL is the API, ultimate efficiency

---

## Core Features

### 🚀 Out-of-the-box, Lightweight

- No coding required, no external dependencies (only needs Java runtime)
- Runs stably on a 2-core 4GB server
- Supports standalone / cluster mode, Windows / Linux

### 🔌 Broad Data Source Compatibility

| Type | Support |
|------|---------|
| **Relational Databases** | MySQL, SQL Server, PostgreSQL, Oracle, Hive, DM, Kingbase, Doris, OceanBase, GaussDB, and **all** JDBC-compatible databases |
| **Elasticsearch** | ES DSL executor, run Elasticsearch queries directly |
| **HTTP Proxy** | HTTP executor, forward third-party REST APIs |

### ✍️ Dynamic SQL, MyBatis-style

- Supports `#{}` / `${}` parameter binding, full MyBatis dynamic SQL syntax
- SQL editor with built-in **run / debug** — WYSIWYG
- Supports Select / Insert / Update / Delete and stored procedures
- Multi-SQL combined execution with flexible transaction control

### 🔄 API Orchestration

- **DAG visual canvas**: drag-and-drop orchestration, no coding required
- Supports Start → API Execution → Condition (If/Else) → End nodes
- Previous API results feed directly into subsequent steps
- Groovy script processing for flexible data handling

### 🛡️ Enterprise-grade Security

| Capability | Description |
|------------|-------------|
| **Dynamic Auth** | clientId + secret to obtain Token, API-level access control |
| **IP Firewall** | IP whitelist / blacklist filtering |
| **Rate Limiting** | API-level QPS throttling |
| **Data Encryption** | RSA encryption for response data, digital signature for request params |
| **Audit Logging** | Full operation audit trail |

### 🧩 Plugin System (5 categories)

- **Cache plugins** — Redis / Ehcache / ES etc.
- **Data transformation plugins** — data masking, format restructuring
- **Alert plugins** — Email, SMS, DingTalk, Feishu, WeCom
- **Parameter processing plugins** — parameter decryption, validation, transformation
- **Global data transformation plugins** — compatible with AMIS and other frontend frameworks

### 🤖 AI + MCP Support

- Map DBAPI data APIs to **MCP tools**
- Integrate with Claude Desktop, Cursor, LangChain, Spring AI and other AI clients
- AI assistant support, generate SQL from natural language

### 📊 Monitoring & Logging

- API call history query & access statistics
- Log storage: ClickHouse / MySQL / PostgreSQL / Doris
- Kafka buffer collection for large-scale scenarios

### 🛠️ More Capabilities

- Dynamic API creation / modification / deactivation, **zero-downtime hot deployment**
- API group management, import/export, version rollback (Enterprise)
- Built-in API variables `__clientId`, `__apiId`
- OpenAPI interface for easy system integration
- Data source health checks, preset request test parameters

---

## Quick Start

### 1. Prerequisites

- JDK 8 / 11 / 17
- OpenSSL 3 (not required on Windows)

### 2. Download & Start

```bash
# Download Community Edition (free)
wget https://img.51dbapi.com/dbapi/dbapi-4.0.32-bin.tar.gz
tar -xzf dbapi-4.0.32-bin.tar.gz
cd dbapi-4.0.32

# Modify database config (default uses embedded SQLite)
# vim conf/application.properties

# Start service
bash bin/dbapi-daemon.sh start standalone
```

### 3. Access the System

Open `http://<your-ip>:8520` in your browser, default credentials `admin / admin`.

> For detailed installation guide see [📖 Installation Guide](https://www.51dbapi.com/en/install)

---

## Live Demo

- **Demo environment**: [https://www.51dbapi.com/demo](https://www.51dbapi.com/demo) (credentials: `admin / admin`)

---

## Community

- **GitHub**: [https://github.com/freakchick/DBApi](https://github.com/freakchick/DBApi)
- **Website**: [https://www.51dbapi.com/en](https://www.51dbapi.com/en)
- **Docs**: [https://www.51dbapi.com/en](https://www.51dbapi.com/en)

---

*If DBAPI helps you, feel free to give the project a ⭐ on GitHub!*
