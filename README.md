# 小娜NAS系统 (AgentNAS / OpenNaNAS)

> 🏠 **天生内嵌小娜助手的AI原生NAS系统**
> 
> *由Agent驱动、AI赋能的下一代网络存储系统*

---

## 🎯 项目愿景

打造全球首款**AI原生、Agent驱动**的开源NAS操作系统，让NAS不仅是存储设备，更是智能家庭/办公的AI中枢。

### 核心理念
- **AI原生**: 从底层设计就融入AI能力，而非后期插件
- **Agent驱动**: 多Agent协作，自动化运维和任务执行
- **轻量易用**: Debian轻量底层 + 直觉化Web界面
- **集群能力**: 支持多节点协同，分布式存储和计算

---

## 🏗️ 系统架构

```
┌─────────────────────────────────────────┐
│        小娜NAS系统 (AgentNAS)            │
│         "小娜助手，您的智能NAS管家"       │
├─────────────────────────────────────────┤
│                                         │
│  【AI交互层】WebGUI + 小娜助手           │
│  ├─ 🎨 现代化文件管理器                 │
│  ├─ 🤖 小娜AI助手对话框                 │
│  ├─ 📊 Agent集群管理面板                │
│  ├─ 🔐 可视化权限配置中心               │
│  └─ 📈 系统监控大屏                     │
│                                         │
├─────────────────────────────────────────┤
│                                         │
│  【智能中台】OpenClaw + Agent系统        │
│  ├─ 🧠 小娜核心 (AI推理引擎)            │
│  ├─ 🔄 Agent协调器 (任务调度)           │
│  ├─ 📡 MQTT消息总线                     │
│  ├─ 🔑 权限引擎 (RBAC/ABAC)             │
│  └─ 🗄️ 知识图谱 (共享记忆)              │
│                                         │
├─────────────────────────────────────────┤
│                                         │
│  【系统服务层】                          │
│  ├─ 💾 分布式存储 (Btrfs/ZFS)           │
│  ├─ 🐳 容器服务 (Docker/Podman)         │
│  ├─ 🌐 网络虚拟化 (OVS/Bridge)          │
│  ├─ 🔒 安全服务 (Firewall/SELinux)      │
│  └─ 📦 应用商店 (Agent技能市场)         │
│                                         │
├─────────────────────────────────────────┤
│                                         │
│  【Debian 12 轻量底层】                  │
│  ├─ 🐧 精简内核 (NAS优化)               │
│  ├─ ⚡ 快速启动 (<30秒)                 │
│  └─ 🔧 硬件抽象 (ARM/x86)               │
│                                         │
└─────────────────────────────────────────┘
```

---

## ✨ 核心特性

### 1. 🤖 小娜AI助手 (内置)
- **自然语言控制**: "小娜，帮我把下载的电影整理到媒体库"
- **智能问答**: "今天谁访问了共享文件夹？"
- **故障诊断**: 自动分析问题并给出修复建议
- **任务自动化**: 学习用户习惯，自动执行常规任务

### 2. 🎭 Agent角色系统
| 角色 | 职责 | 代表 |
|------|------|------|
| **治理层** | 架构设计、规则制定、审批 | Nova |
| **救援层** | 系统维护、故障修复、监控 | 小娜(NANA) |
| **任务层** | 项目执行、代码开发、文件整理 | 伊伊、橘子 |

### 3. 🏠 智能文件管理
- **AI自动分类**: 照片/视频/文档自动归类
- **语义搜索**: "找去年夏天的海边照片"
- **智能标签**: AI自动提取内容标签
- **重复文件检测**: 基于内容的去重

### 4. 🔐 企业级权限
- **RBAC角色权限**: 治理/救援/任务三层架构
- **细粒度控制**: 文件级、服务级、Agent级权限
- **审计日志**: 所有操作可追溯
- **多租户隔离**: 家庭/团队场景支持

### 5. 🌐 集群协同
- **多节点管理**: 一个界面管理所有NAS节点
- **分布式存储**: 多节点冗余，高可用
- **负载均衡**: 任务自动分配到空闲节点
- **故障转移**: 节点故障自动切换

---

## 🛠️ 技术栈

### 前端 (WebGUI)
- **Vue 3** + TypeScript - 响应式框架
- **Naive UI** - 现代化组件库
- **ECharts** - 数据可视化
- **WebSocket** - 实时通信

### 后端 (API服务)
- **Go** (Gin) - 高性能API Gateway
- **Node.js** - OpenClaw/Agent集成
- **PostgreSQL** - 配置数据库
- **Redis** - 缓存与消息队列
- **MQTT** (Mosquitto) - Agent通信

### 系统层
- **Debian 12** - 轻量基础系统
- **Btrfs/ZFS** - 高级文件系统
- **Docker** - 容器化运行
- **systemd** - 服务管理

---

## 📋 功能

- [ ] Debian 12轻量镜像定制
- [ ] 基础WebGUI框架
- [ ] 文件管理核心功能
- [ ] 小娜助手基础对话
- [ ] 单节点存储管理
- [ ] Agent角色系统
- [ ] 权限管理(RBAC)
- [ ] AI文件分类/搜索
- [ ] 自动化任务流
- [ ] 应用商店
- [ ] 多节点管理
- [ ] 分布式存储
- [ ] 集群监控
- [ ] 故障自动恢复
- [ ] 远程访问
- [ ] 技能市场
- [ ] 第三方集成
- [ ] 硬件适配
- [ ] 社区生态

---

## 🚀 快速开始

### 安装要求
- **硬件**: ARM64/x86_64, 2GB+ RAM, 16GB+ 存储
- **网络**: 有网络连接 (可选)
- **设备**: 树莓派/迷你主机/旧电脑/NAS设备

### 安装方式

#### 方式一: ISO镜像安装 (推荐)
```bash
# 下载ISO镜像
wget https://github.com/opennanas/agentnas/releases/download/v1.0/agentnas-v1.0-amd64.iso

# 制作启动盘 (Linux/Mac)
dd if=agentnas-v1.0-amd64.iso of=/dev/sdX bs=4M

# 启动安装
# 按向导完成安装
```

#### 方式二: Docker运行
```bash
docker run -d \
  --name agentnas \
  --privileged \
  -p 80:80 \
  -p 443:443 \
  -v /path/to/data:/data \
  agentnas/agentnas:latest
```

#### 方式三: 现有Debian系统安装
```bash
# 一键安装脚本
curl -fsSL https://get.agentnas.io | bash
```

### 首次配置
1. 浏览器访问 `http://设备IP`
2. 创建管理员账号 (默认: admin/admin)
3. 初始化存储池
4. 邀请小娜助手: "小娜，你好！"

---

## 📚 文档

- [快速入门](docs/quickstart.md)
- [架构设计](AgentNAS-架构设计.md) ← 核心技术文档
- [开发路线图](AgentNAS-开发路线图.md) ← 项目规划
- [开发指南](docs/development.md)
- [API文档](docs/api.md)
- [常见问题](docs/faq.md)

---

## 🤝 参与贡献

我们欢迎所有形式的贡献！

### 贡献方式
- 🐛 [提交Bug](https://github.com/opennanas/agentnas/issues)
- 💡 [提出建议](https://github.com/opennanas/agentnas/discussions)
- 📝 [完善文档](https://github.com/opennanas/agentnas/tree/main/docs)
- 💻 [提交代码](https://github.com/opennanas/agentnas/pulls)

### 开发环境搭建
```bash
# 克隆仓库
git clone https://github.com/opennanas/agentnas.git
cd agentnas

# 安装依赖
npm install  # 前端
go mod tidy  # 后端

# 启动开发服务器
make dev
```

---

## 📄 许可证

[GPL-3.0](LICENSE) © 2026 AgentNAS Team

---

## 🙏 致谢

- [OpenClaw](https://github.com/openclaw/openclaw) - Agent系统基础
- [Debian](https://www.debian.org/) - 可靠的操作系统基础
- [FNOS](https://www.fnos.com/) - NAS交互设计灵感
- [所有贡献者](CONTRIBUTORS.md)

---

> 💬 **小娜说**: "我是小娜，您的智能NAS管家！有任何问题随时问我哦~"

**[⬆ 回到顶部](#小娜NAS系统-agentnas--opennanas)**
