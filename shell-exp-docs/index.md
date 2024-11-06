---
title: What is a command shell?
ms.date: 11/06/2024
description: Learn what a command shell is and how it works.
---
# What is a command shell?

A command shell is a text-based interface for interacting with a computer, also known as a
Read-Eval-Print Loop ([REPL](https://wikipedia.org/wiki/Read%E2%80%93eval%E2%80%93print_loop)).

A shell takes input from the keyboard, evaluates that input, and executes the input as a shell
command or gives the input to the operating system to be executed. Most shells can also read
commands from a script file, and may include programming features like variables, flow control, and
functions.

## Terminals

- [Windows Terminal](/windows/terminal)
- [Terminal for macOS](https://support.apple.com/guide/terminal/welcome/mac)
- [iTerm2 for macOS](https://iterm2.com/)
- [Cloud Shell](/azure/cloud-shell/overview)

## General purpose command shells

General purpose command shells are designed to work with the operating system. These shell allow you
to run any command that the operating system supports. They also include shell-specific commands and
programming features.

- [PowerShell](/powershell/scripting/overview)
- [Windows Command Shell](/windows-server/administration/windows-commands/cmd)
- [bash](https://www.gnu.org/software/bash/) - popluar on Linux
- [zsh](https://support.apple.com/102360) - popluar on macOS

## Utility command shells

Utility command shells are designed to work with specific applications or services. These shells can
only run commands that are specific to the application or service. Some utility shells support
running commands from a script file, but they don't include programming features. Usually, these
shells can only be used interactively.

- [AIShell](aishell/overview.md) - An interactive-only shell used to communicate with AI services
  such as Azure OpenAI.
- [netsh](/windows-server/administration/windows-commands/netsh) - Network shell (netsh) is a
  command-line utility that allows you to configure and display the status of various network
  components on Windows. It is both a command-line tool and a command shell. It also supports
  running commands from a script file.

## Command-line tools

A command-line tool is a standalone program that is run from a command shell. Command-line tools are
typically designed to perform a specific task, such as managing files, configuring settings, or
querying for information. Command-line tools can be used in any shell that supports running external
programs.

- [Azure CLI](/cli/azure) - a collection of command-line tools for managing Azure resources that can
  be run in any supported shell.
- [Azure PowerShell](/powershell/azure) - a collection of PowerShell modules for managing Azure
  resources that can be run in any supported version of PowerShell.
- [OpenSSH for Windows](/windows-server/administration/openssh/openssh-overview) - a command-line
  client, as well as a server, for secure communication over a network.
- [Windows Commands](/windows-server/administration/windows-commands/windows-commands) - a
  collection of command-line tools that are built into Windows.

In general, command-line tools don't provide a command shell (REPL) interface. The `netsh` command
in Windows is an exception, as it is both a command-line tool and a an interactive command shell.
