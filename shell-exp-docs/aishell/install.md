---
title: Install AIShell
description: Learn how to install AIShell on your system.
ms.date: 10/29/2024
---
# Install AIShell

AIShell is an interactive shell that provides a chat interface with language models. There are
packages you need to install to have a complete AIShell experience.

- The command-line shell (`aish`) interface
- The AIShell module for PowerShell

This article explains how to install these packages on your system.

## System requirements

AIShell is supported on the following platforms:

<!-- markdownlint-disable MD023 MD024 MD051 -->
### [Windows](#tab/windows)

Windows

- Windows 10 or higher
- PowerShell 7.4 or higher
- Windows Terminal

### [macOS](#tab/macos)

macOS

- macOS v13 Ventura or higher
- PowerShell 7.4 or higher
- iTerm2

### [Linux](#tab/linux)

Linux

- Ubuntu 20.04 or higher
- PowerShell 7.4 or higher (recommended)
- Any terminal emulator supported by the OS

  > [!NOTE]
  > The AIShell module isn't supported on Linux.

<!-- markdownlint-enable MD023 MD024 MD051 -->

---

## Install AIShell

<!-- markdownlint-disable MD023 MD024 MD051 -->
### [Windows](#tab/windows)

1. Download the latest version from the
   [GitHub releases page](https://github.com/PowerShell/ProjectMercury/releases/latest).
1. Install the AIShell module from the PowerShell Gallery.

   ```powershell
   Install-PSResource -Name AIShell
   ```

### [macOS](#tab/macos)

1. Insert brew steps here.
1. Install the AIShell module from the PowerShell Gallery.

   ```powershell
   Install-PSResource -Name AIShell
   ```

### [Linux](#tab/linux)

1. Insert Linux steps here.

<!-- markdownlint-enable MD023 MD024 MD051 -->

---

## Next steps

- [Get started with AIShell](get-started-standalone.md)
- [Get started with AIShell for PowerShell](get-started-powershell.md)
