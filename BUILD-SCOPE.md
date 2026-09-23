# Public Build Scope

## Included

- Unity C# scripts for Lua/UI adaptation.
- Unity `.meta` files for the published scripts.
- C++ asynchronous callback examples.
- Product screenshots and documentation.

## Not present as a complete public build

The repository does not currently contain a complete Unity `Assets` tree, `Packages/manifest.json`, `ProjectSettings`, generated C++ protocol headers, all linked server libraries, database schema, production configuration, or a verified one-command deployment definition.

Treat this repository as a source reference package. Do not advertise `docker compose up`, a standalone CMake build, or production concurrency figures until the corresponding files and reproducible results are committed.

## Checklist for future buildable releases

1. Record exact Unity or compiler versions.
2. Record operating system and dependency versions.
3. Test commands from a clean checkout.
4. Publish artifact names and checksums.
5. Record a login and lobby smoke test.
6. List known limitations and excluded services.

