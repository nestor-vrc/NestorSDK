# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.1.0] - 2024-10-19

### Added

- **CopyBlendShape Tool**: Added a utility to copy blend shapes between GameObjects in Unity.
- **UnbanUser Utility**: Implemented a utility to clear the `DefaultCompany` temp directory. Added confirmation dialogs for safer operations.

### Changed

- **Config Management**: Refactored config loading in `NestorConfig` to improve performance using a static `HttpClient` instance.
- **Discord RPC**: Improved error handling, logging, and renamed config variables for better clarity.
- **Blend Shape Tool**: Updated blend shape copying methods to instance context and improved validation logic.

### Fixed

- **Thumbnail Keyword Conflict**: Escaped reserved keyword `value` in `ThumbnailFoldout.cs` to avoid shader property conflicts.
- **Upload issue**: Fixed SceneManagement namespace error. Updated SceneSaver to include UnityEditor.SceneManagement conditionally with #if UNITY_EDITOR

---

## [0.0.1] - 2024-10-03

### Added

- **Nestor SDK**: Introduced the Nestor SDK with Discord RPC integration and configuration system.
- **VRChat Creator Companion**: Added support for VRChat Creator Companion (VCC) with VRChat avatars and base package as Nestor SDK base.

### Changed

- **Menu Items**: Updated VRChat references in menu items to Nestor SDK.
- **Configuration Handling**: Improved the structure and readability of configuration classes in the Nestor SDK.
  
### Fixed

- **Validation Checks**: Restored validation functionality for avatar performance checks by removing temporary bypasses.
- **File Organization**: Refactored various files for better readability and maintainability, including updates to dependencies and configurations.

### Removed

- **Unused Resources**: Deleted outdated images and UXML files from the SDK panel.
- **Shader Validation**: Bypassed shader validation and stripping for mobile platforms in SDK builders, Can be uploaded but cannot be verified.
