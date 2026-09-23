# 德州扑克金币大厅源码｜Unity + Lua UI 与 C++ 登录回调

> Texas Holdem Game Source Code · 德州源码 · 德州撲克源碼 · Poker Lobby Source Code

[简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md) | [图文产品页](https://niubideren111.github.io/Texas-Holdem-Game-Source-Code/zh-cn/)

这是一个面向**德州扑克金币大厅、移动端登录和玩法入口**的公开源码资料仓库。仓库提供 Unity C# / Lua UI 适配器、签名工具、C++ 异步登录与用户状态回调，以及可核对的产品界面截图，适合研究德州扑克客户端 UI 桥接和服务端回调结构。

![德州扑克金币大厅活动界面](docs/assets/seo/texas-holdem-game-source-code-01.jpg)

## 项目亮点

- **完整德州扑克产品形态**：从账号登录、金币大厅、玩法选场到牌桌对局，覆盖移动端玩家的主要使用流程。
- **大厅与多玩法入口**：展示金币场、SNG、MTT、私人局和俱乐部等产品入口与买入档位设计。
- **Unity + Lua UI 架构**：通过 C# Adapter 连接 Lua 业务界面，适合大厅列表、牌桌列表和活动页面扩展。
- **C++ 异步服务回调**：提供登录、登出、用户信息、用户状态和服务器映射回调参考。
- **真实产品截图**：公开登录、金币大厅活动和 SNG 选场界面，便于评估产品风格与交互结构。
- **多语言资料**：提供简体中文、繁体中文和英文 README 与 GitHub Pages 产品页。

## 核心功能

| 功能模块 | 产品能力 |
|---|---|
| **账号与登录** | 手机号登录、用户状态处理、登录与登出异步回调 |
| **金币大厅** | 多级别选场、买入档位、快速进入牌桌和大厅活动入口 |
| **经典德州** | 玩家入桌、下注、跟注、加注、弃牌、All-in 和结算流程 |
| **私人局 / 朋友局** | 好友组局、自定义牌桌参数和房间入口 |
| **俱乐部体系** | 俱乐部牌桌、成员组局、战绩与社交入口 |
| **SNG / MTT** | 单桌赛、多桌锦标赛、选场和报名买入界面 |
| **特色玩法入口** | 产品资料展示短牌、奥马哈等玩法扩展方向 |
| **活动与奖励** | 宝箱、福利活动和大厅运营入口 |
| **社交体验** | 好友、聊天、表情及牌桌互动的产品扩展空间 |
| **多语言与多端** | Unity 移动端架构，可用于 Android/iOS 客户端适配研究 |

## 核心特色

1. **面向真实移动端大厅体验**：界面不是单一牌型 Demo，而是包含登录、选场、活动和赛事入口的完整产品设计参考。
2. **客户端与服务端资料并列**：既有 Unity/Lua UI 适配代码，也有 C++ 用户服务回调，便于理解前后端衔接。
3. **适合二次开发评估**：源码地图明确标出每个公开文件的职责，可快速判断哪些模块能够复用。
4. **功能描述与公开范围分离**：上表说明产品展示能力；实际公开代码覆盖程度以“公开源码地图”和 `BUILD-SCOPE.md` 为准。

## 产品截图

| 金币大厅活动 | SNG 选场与买入 | 手机号登录 |
|---|---|---|
| ![德州扑克金币大厅宝箱活动](docs/assets/seo/texas-holdem-game-source-code-01.jpg) | ![德州扑克 SNG 选场和买入档位](docs/assets/seo/texas-holdem-game-source-code-02.jpg) | ![德州扑克移动端手机号登录](docs/assets/seo/texas-holdem-game-source-code-03.jpg) |

## 公开源码地图

| 路径 | 内容 |
|---|---|
| [`LuaUIObject.cs`](LuaUIObject.cs) | Lua UI 对象桥接 |
| [`LuaOSAListAdapter.cs`](LuaOSAListAdapter.cs) | Lua 列表适配器 |
| [`LuaOSATableAdapter.cs`](LuaOSATableAdapter.cs) | Lua 表格适配器 |
| [`SignatureTool.cs`](SignatureTool.cs) | 客户端签名辅助工具 |
| [`external/AsyncLoginCallback.cpp`](external/AsyncLoginCallback.cpp) | C++ 异步登录回调 |
| [`external/AsyncGetUserCallback.cpp`](external/AsyncGetUserCallback.cpp) | 用户信息回调 |
| [`external/AsyncUserServerMapCallback.cpp`](external/AsyncUserServerMapCallback.cpp) | 用户服务器映射回调 |

完整说明见 [SOURCE-MAP.md](SOURCE-MAP.md)。

## 适合谁阅读

- 研究 Unity 德州扑克大厅 UI 的开发者。
- 需要了解 C# 与 Lua UI 适配方式的客户端工程师。
- 需要参考 C++ 异步登录和用户状态回调的服务端工程师。
- 评估金币大厅、登录流程和 SNG 入口的产品人员。

## 开始阅读

```bash
git clone https://github.com/niubideren111/Texas-Holdem-Game-Source-Code.git
cd Texas-Holdem-Game-Source-Code
```

建议先查看截图，再依次阅读 `LuaUIObject.cs`、两个 OSA Adapter 和 `external/AsyncLoginCallback.cpp`。构建前请阅读 [BUILD-SCOPE.md](BUILD-SCOPE.md)。

## 公开范围说明

当前公开仓库是**可阅读的源码与产品资料集合**，并非包含全部 Unity Assets、完整服务集群、数据库脚本和生产配置的一键部署工程。因此不承诺通过 Docker、CMake 或单条命令即可启动完整游戏。

## 与其他项目的区别

- 本仓库：金币大厅、登录、SNG 入口、Unity/Lua UI 与登录回调。
- [德州私人局与朋友局源码](https://github.com/niubideren111/Texas-Hold-em-source-code)：私人房间和朋友组局。
- [德州俱乐部源码](https://github.com/niubideren111/dezhou-poker-club-source-code)：俱乐部、联盟和牌桌。
- [德州锦标赛源码](https://github.com/niubideren111/Texas-Hold-em-Tournament-Source-Code)：MTT、SNG 和比赛资料。

## 常见问题

### 这是完整可运行的德州扑克项目吗？

公开仓库包含 UI 适配器、工具类、服务端回调片段和产品截图。可独立构建范围以 [BUILD-SCOPE.md](BUILD-SCOPE.md) 为准。

### 这是德州俱乐部源码吗？

本仓库主要展示金币大厅和玩法入口。俱乐部需求请访问上方独立仓库，以减少同账号项目间的关键词竞争。

## 文档、许可与联系

- [源码地图](SOURCE-MAP.md)
- [公开范围与构建条件](BUILD-SCOPE.md)
- [贡献说明](CONTRIBUTING.md)
- [安全说明](SECURITY.md)
- [许可证](LICENSE)

本项目用于软件工程学习、架构研究和合法二次开发。涉及线上服务、支付或用户数据时，请遵守适用法律、平台规则和隐私要求。

Telegram: [@fox_lovemyself](https://t.me/fox_lovemyself) · GitHub: [niubideren111](https://github.com/niubideren111)
