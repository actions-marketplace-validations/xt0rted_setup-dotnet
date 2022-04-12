# Changelog

## Unreleased

## 1.0.0

- Use `actions/setup-dotnet` 2.0.0
- Set `DOTNET_INSTALL_DIR` based on the OS.
  - Prevents pre-installed SDKs from being downloaded and installed a second time.
  - Fixes the issue of losing access to pre-installed SDKs after installing a new one.
- Strip comments from the `global.json` so `actions/setup-dotnet` can read the SDK version from it.