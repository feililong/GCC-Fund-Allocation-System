# GCC公共资金分配自动化系统

基于多 Agent 协同架构的智能资金分配系统，为公共物品基金提供里程碑多源核验、链上自动拨付、多渠道状态通知全流程自动化。

## 核心特性

- **多源里程碑核验**：自动对接 GitHub、链上数据、IPFS 等多源验证，置信度评分机制
- **链上自动拨付**：集成 Gnosis Safe 多签钱包，支持 Ethereum、Polygon、Arbitrum 等 6 条公链
- **智能状态通知**：Telegram、Discord、邮件多渠道同步，支持自定义规则
- **全程可审计**：所有操作存证 IPFS，自动生成审计报告
- **模块化设计**：四个独立 Agent 可单独部署，支持灵活组合

## 快速开始

### 环境要求

- Node.js 18+
- PostgreSQL 14+
- Redis 7+
- Docker & Docker Compose

### Docker 部署

```bash
# 克隆仓库
git clone https://github.com/GCCofCommons/fund-allocation-system.git
cd fund-allocation-system

# 配置环境变量
cp .env.example .env
# 编辑 .env 文件，填入必要的配置

# 启动服务
docker-compose up -d

# 查看日志
docker-compose logs -f
