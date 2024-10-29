---
title: What is AIShell?
description: Learn about AIShell, an interactive shell that provides a chat interface with language models.
ms.date: 10/29/2024
---

# What is AIShell?

AIShell is an interactive shell that provides a chat interface with language models. The shell
provides agents that connect to different AI models and other assistance providers. Users can
interact with the agents in a conversational manner.

The AIShell project includes:

- The command-line shell (`aish`) interface
- A framework for creating AI agents and other assistance providers
- Integration with Windows Terminal and iTerm2 on macOS
- A PowerShell module for tight integration with PowerShell. For more information, see the
  [AIShell module][01].

Each AI assistant is known as an agent. The initial release of AIShell includes two agents:

- **Azure OpenAI** agent that connects to an instance of **gpt-4o**. Use this agent for general
  AI tasks.
- **Azure command** agent that can assist with Azure CLI commands. Use the Azure agent for
  assistance with Azure CLI and Azure PowerShell commands.

The AIShell executable (`aish.exe`) can be run in a standalone experience or in split-screen mode if
you're using Windows Terminal or iTerm2 macOS. You can use the **AIShell** PowerShell module with
PowerShell 7 to create a split-screen experience. This is the recommended way to use AIShell because
you get deeper integration with the shell. These features include:

- Inserting code from the sidecar response directly into the working shell
- Multi-step commands are put into the Predictive IntelliSense buffer for quick acceptance
- Simple, single-command error recovery

<!-- link references -->
[01]: /powershell/utility-modules/aishell/overview
