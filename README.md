# 德州扑克源码（德州源码）｜金币大厅、多玩法与 Unity UI 资料|Texas Hold'em Poker Source Code

> 中文简体 · 中文繁體 · English 多语言产品与源码资料

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [English](README.en.md) · [产品页面](https://niubideren111.github.io/Texas-Holdem-Game-Source-Code/zh-cn/)

以金币大厅和多玩法入口为主题的德州扑克项目资料，展示登录、SNG 选场和宝箱等界面。公开代码包含 Unity C# 与 Lua UI 适配器、签名工具和服务器异步回调片段。

**德州扑克源码 · 德州源码 · 德州金币大厅源码 · Unity扑克源码**
支持经典德州、短牌、奥马哈等多种玩法，包含私人局、朋友局、俱乐部/联盟、SNG、MTT 等模式。

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Stars](https://img.shields.io/github/stars/niubideren111/Texas-Hold-em-source-code)](https://github.com/niubideren111/Texas-Hold-em-source-code/stargazers)

---

## ✨ 项目亮点

- **服务器权威架构**：所有核心逻辑（发牌、胜负判定、行为验证）均在服务端执行，有效防止外挂与作弊
- **高并发低延迟**：基于 WebSocket 实时通信，支持数百人同时在线对战
- **多玩法支持**：经典德州（9人/6人桌）、短牌、奥马哈等
- **丰富模式**：金币场、私人局、朋友局、俱乐部、联盟、SNG、MTT 锦标赛
- **AI 机器人**：内置智能 Bot，便于测试与桌位填充
- **技术栈**：C++ 高性能服务端 + Unity 2019+ 客户端 + MySQL + Redis + Docker

> **重要声明**：本项目**仅供学习、研究和二次开发使用**。严格禁止用于任何真实货币赌博活动。商业使用请严格遵守当地法律法规，作者不承担任何法律责任。

---

## 📖 目录

- [快速开始](#快速开始)
- [核心功能](#核心功能)
- [技术架构](#技术架构)
- [二次开发建议](#二次开发建议)
- [未来路线图](#未来路线图)
- [联系方式](#联系方式)

---

## 🚀 快速开始

### Docker 一键部署（推荐）


git clone https://github.com/niubideren111/Texas-Hold-em-source-code.git
cd Texas-Hold-em-source-code
docker-compose up -d

源码编译运行（Linux）
mkdir build && cd build
cmake .. -DCMAKE_BUILD_TYPE=Release
make -j$(nproc)
./poker_server
---

## ✨ Features | 核心功能 | 功能特色

* ✅ Texas Hold'em gameplay ｜ 德州玩法 ｜ 德州玩法
* ✅ Multiplayer real-time ｜ 实时对战 ｜ 即時對戰
* ✅ Table management ｜ 牌桌管理 ｜ 牌桌管理
* ✅ Stable game server ｜ 稳定服务端 ｜ 穩定服務端
* ✅ Scalable architecture ｜ 可扩展 ｜ 可擴展
* ✅ High-performance engine ｜ 高性能引擎 ｜ 高效能引擎
* ✅模块主要功能金币大厅快速匹配、多级别桌、坐满即玩、
* ✅每日比赛俱乐部/私人局好友约局、俱乐部管理、战绩统计、联盟系统
* ✅锦标赛系统SNG、MTT、多桌锦标赛、赏金赛特色玩法
* ✅经典德州、短牌、奥马哈等社交系统
* ✅语音聊天、好友系统、表情互动
* ✅安全与日志服务器反作弊、完整行为日志、数据分析
## 💰 Commercial Features | 商业能力 | 商業能力

- ✔ Payment & recharge system（充值系统）  
- ✔ Multi-language support（多语言支持）  
- ✔ Multi-currency support（多货币支持）  
- ✔ Referral / agent system（代理体系）  
- ✔ Player interaction & chat（互动聊天） 
---
##🛠 技术架构

服务端：C++ 高并发框架（WebSocket）
客户端：Unity 2019+（C#），支持 Android / iOS / PC
数据库：MySQL（持久化） + Redis（缓存、实时数据）
部署：Docker + docker-compose，支持水平扩展
通信协议：WebSocket（二进制/JSON 可选）

---


###📈 未来路线图

  * 完善 SNG/MTT 完整锦标赛流程
  * 支持更多扑克变体（奥马哈 Hi/Lo 等） 
  *  分布式部署与 Redis Cluster 集成 
  *  WebGL / HTML5 客户端示例 
 *  更完善的后台管理系统 

## 项目咨询

- Telegram：[fox_lovemyself](https://t.me/fox_lovemyself)
- GitHub：[德州私人局与朋友局源码](https://github.com/niubideren111/Texas-Hold-em-source-code)



## 📸 Screenshots | 项目展示 | 專案展示

![德州扑克金币大厅宝箱活动界面](docs/assets/seo/texas-holdem-game-source-code-01.jpg)

![德州扑克 SNG 选场与买入档位](docs/assets/seo/texas-holdem-game-source-code-02.jpg)

![德州扑克手机号登录界面](docs/assets/seo/texas-holdem-game-source-code-03.jpg)

---
## 公开源码与资料

| 文件 | 说明 |
|---|---|
| [LuaOSAListAdapter.cs](LuaOSAListAdapter.cs) | Lua 列表适配器 |
| [LuaOSATableAdapter.cs](LuaOSATableAdapter.cs) | Lua 表格适配器 |
| [LuaUIObject.cs](LuaUIObject.cs) | Lua UI 对象桥接 |
| [SignatureTool.cs](SignatureTool.cs) | 签名工具类 |
| [external/AsyncLoginCallback.cpp](external/AsyncLoginCallback.cpp) | 服务端登录回调片段 |

## 获取仓库

```bash
git clone https://github.com/niubideren111/Texas-Hold-em-source-code.git
cd Texas-Hold-em-source-code
```

克隆后从上面的文件入口开始阅读。若需要运行示例，请先核对项目中实际存在的依赖、版本、配置和启动脚本。

## 常见问题

### 本项目与私人局项目有何不同？

本页突出金币大厅、玩法选择和 Unity UI 代码；私人局项目侧重组局、俱乐部牌桌和场景资料。

### 从哪个文件了解客户端界面？

从 LuaUIObject.cs 入手，再阅读列表和表格适配器，了解 C# 与 Lua 界面的连接方式。

## 后续资料完善方向

补充登录到大厅的流程图、玩法入口截图、UI 适配器用法和 Unity 版本说明；独立列出 SNG/MTT 的实现范围。 后续更新还应加入版本化依赖清单、经过验证的构建或导入步骤、简明架构/产品流程图，以及能对应真实文件变化的版本记录。大型授权资源可放入 GitHub Releases 并提供校验值，不能提交密钥、生产地址或用户数据。

## 相关项目

- [Texas-Hold-em-source-code](https://github.com/niubideren111/Texas-Hold-em-source-code)
- [dezhou-poker-club-source-code](https://github.com/niubideren111/dezhou-poker-club-source-code)
- [Texas-Hold-em-Tournament-Source-Code](https://github.com/niubideren111/Texas-Hold-em-Tournament-Source-Code)

## 资料范围与许可

公开仓库提供 UI 适配代码、工具类、服务器回调片段及产品截图；完整客户端、服务端和数据配置通过项目联系方式沟通。 公开内容以实际文件、依赖和许可为准，不承诺搜索排名、直接上线或固定性能结果。

- Telegram: [@fox_lovemyself](https://t.me/fox_lovemyself)
- GitHub: [Texas-Holdem-Game-Source-Code](https://github.com/niubideren111/Texas-Holdem-Game-Source-Code)

