---
title: What is AIShell?
description: Learn about AIShell, an interactive shell that provides a chat interface with language models.
ms.date: 10/29/2024
ms.topic: overview
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
- **Copilot in Azure** agent that can assist with Microsoft Azure knowledge. Use the Azure agent for
  assistance with Azure CLI and Azure PowerShell commands.

The AIShell executable (`aish.exe`) can be run in a standalone experience or in split-screen mode if
you're using Windows Terminal or iTerm2 macOS. You can use the **AIShell** PowerShell module with
PowerShell 7 to create a split-screen experience. This is the recommended way to use AIShell because
you get deeper integration with the shell. These features include:

- Inserting code from the sidecar response directly into the working shell
- Multi-step commands are put into the Predictive IntelliSense buffer for quick acceptance
- Simple, single-command error recovery

# Project Status

AIShell is currently in **Public Preview**. This means that the tool is available for testing, but
it is not yet fully feature-complete. While AIShell is functional, please note that some elements of
the tool are still under development and may be subject to change. Your feedback is invaluable to us
during this phase, and we encourage users to share their experiences to help us improve AIShell.

## Known Issues
As AIShell is still in its preview phase, there are some known issues that we are actively working
on addressing. Below are placeholders for current known issues. Check back frequently for updates:

- The PowerShell module to enable the sidecar experience is not supported on Linux and is limitedly supported on Mac. The `aish`
  executable can be run on Linux, but the sidecar experience is not available. 
- When using `Start-AIShell` and you have multiple versions of Windows Terminal installed or when
  running as an administrator, the command will open a different window/version of Windows Terminal.

If you encounter any additional issues that aren’t listed here, please don’t hesitate to report them.

# Providing Feedback and Contributing

## Providing Feedback
To share your feedback, please use the following channels:
- **GitHub Issues:** Open an issue on the [GitHub repo][02] to provide detailed feedback on bugs or request new features.
- **GitHub Community Discussions:** Join our community discussions, where you can share ideas, discuss potential improvements, and connect with other users. Links to our community pages can be found on the [GitHub discussions tab][03].

## How to Contribute
We welcome contributions to help improve AIShell! Here are ways you can get involved:

- **File Issues:** If you encounter bugs, have suggestions for new features, or would like to report inconsistencies, please open an issue on the [AIShell GitHub repository][02].
- **Documentation:** If you notice any documentation gaps, feel free to suggest changes or submit PRs to improve the clarity and usability of our documentation.

We aren't currently accepting pull requests, but we highly value your contributions in other forms.

<!-- link references -->
[01]: /powershell/utility-modules/aishell/overview
[02]: https://github.com/PowerShell/ProjectMercury/issues
[03]: https://github.com/PowerShell/ProjectMercury/discussions
