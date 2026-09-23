# Source Map

This document maps public files to observable purposes.

## Unity and Lua UI

| File | Purpose |
|---|---|
| `LuaUIObject.cs` | Base bridge for Lua-driven Unity UI objects |
| `LuaOSAListAdapter.cs` | Adapter for list-style UI data and recycled views |
| `LuaOSATableAdapter.cs` | Adapter for table-style UI data and recycled views |
| `SignatureTool.cs` | Client-side signature helper |

The matching `.meta` files preserve Unity asset identifiers.

## C++ callback examples

The `external/` directory contains login, logout, user data, user state, assistant service and user-to-server mapping callbacks. These are integration fragments and require matching generated protocol headers, framework libraries and the surrounding server project.

## Product evidence

Images under `docs/assets/seo/` show mobile login, lobby activity UI and SNG selection. Captions describe visible UI and do not claim that every depicted subsystem is included in the public files.

