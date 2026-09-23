# Texas Holdem Game Source Code | Unity Lobby, Lua UI and Multiplayer Materials

[简体中文](README.zh-CN.md) · [繁體中文](README.zh-TW.md) · [English](README.en.md) · [Product page](https://niubideren111.github.io/Texas-Holdem-Game-Source-Code/en/)

A coin-lobby and multi-mode poker project reference with login, SNG and event screens, plus public Unity C#, Lua UI adapters, signing utilities and selected server callbacks.

**Texas Holdem game source code · Unity poker source code · poker lobby source code · multiplayer poker game**

## Project Highlights

- Covers the mobile product flow from login and coin lobby to game selection, promotions and poker tables.
- Presents coin games, private tables, clubs, SNG, MTT and additional poker-mode entry points.
- Uses Unity C# and Lua UI adapters for extensible lobby lists, tables and event screens.
- Includes C++ asynchronous callbacks for login, logout, user data, user state and server mapping.
- Shows real product screens for mobile login, lobby rewards and SNG selection.

## Core Features

| Module | Product capability |
|---|---|
| Account and login | Mobile login, user state, asynchronous login and logout callbacks |
| Coin lobby | Multiple stakes, buy-in tiers, quick table entry and promotion access |
| Texas Holdem | Bet, call, raise, fold, all-in and settlement flow |
| Private games and clubs | Friend tables, club rooms, member and game-history entry points |
| SNG and MTT | Sit-and-go and multi-table tournament selection and registration UI |
| Variant entry points | Product material for Short Deck, Omaha and further extensions |
| Unity/Lua UI | List, table and generic UI-object adapters |
| C++ callbacks | Login, user data, state and user-server mapping callbacks |

This table describes the presented product scope. Public source coverage is documented separately in the source table and `BUILD-SCOPE.md`.

## What this repository presents

### Lobby and game modes

Review login, SNG selection and event screens for the mobile lobby structure.

### Unity and Lua UI

Read list, table and UI-object adapters to understand the C# and Lua bridge.

### Callbacks and utilities

Use login callbacks and SignatureTool.cs as concrete source-code entry points.

## How to evaluate the material

1. **Confirm the product:** review the screenshots and captions to identify the product type and visible workflow.
2. **Inspect the evidence:** open the listed source files or documents instead of relying on feature claims alone.
3. **Check buildability:** verify that required dependencies, assets, configuration and startup scripts are present for the part you intend to run.
4. **Confirm licensing:** read the repository license and obtain written permission for any commercial assets or complete-project delivery.

## Product screenshots

![Texas Holdem coin-lobby event screen](docs/assets/seo/texas-holdem-game-source-code-01.jpg)

![SNG selection and buy-in levels](docs/assets/seo/texas-holdem-game-source-code-02.jpg)

![Mobile-number poker login screen](docs/assets/seo/texas-holdem-game-source-code-03.jpg)

## Public source and documents

| File | Description |
|---|---|
| [LuaOSAListAdapter.cs](LuaOSAListAdapter.cs) | Public CS file: LuaOSAListAdapter.cs. |
| [LuaOSATableAdapter.cs](LuaOSATableAdapter.cs) | Public CS file: LuaOSATableAdapter.cs. |
| [LuaUIObject.cs](LuaUIObject.cs) | Public CS file: LuaUIObject.cs. |
| [SignatureTool.cs](SignatureTool.cs) | Public CS file: SignatureTool.cs. |
| [external/AsyncLoginCallback.cpp](external/AsyncLoginCallback.cpp) | Public CPP file: AsyncLoginCallback.cpp. |

## Start reading

```bash
git clone https://github.com/niubideren111/Texas-Holdem-Game-Source-Code.git
cd Texas-Holdem-Game-Source-Code
```

## Questions

### How does this differ from the private-table repository?

This page focuses on the coin lobby, mode selection and Unity UI; the private-table repository focuses on friend games and club tables.

### Where should I begin with the client UI?

Start with LuaUIObject.cs, followed by the list and table adapters.

## Documentation roadmap

Future updates should add a versioned dependency list, a verified setup or import procedure, a concise architecture or product-flow diagram, and release notes tied to real file changes. Large authorized assets belong in GitHub Releases with checksums; secrets, production endpoints and user data must never be committed.

## Related repositories

- [Texas-Hold-em-source-code](https://github.com/niubideren111/Texas-Hold-em-source-code)
- [dezhou-poker-club-source-code](https://github.com/niubideren111/dezhou-poker-club-source-code)
- [Texas-Hold-em-Tournament-Source-Code](https://github.com/niubideren111/Texas-Hold-em-Tournament-Source-Code)

## Scope and license

The public repository provides UI adapter code, utilities, selected server callbacks and screenshots. Confirm the complete client, server and data configuration separately. Public files should be evaluated against their actual paths, dependencies and license. No search ranking, production readiness or performance result is guaranteed.

- Telegram: [@fox_lovemyself](https://t.me/fox_lovemyself)
- GitHub: [Texas-Holdem-Game-Source-Code](https://github.com/niubideren111/Texas-Holdem-Game-Source-Code)
