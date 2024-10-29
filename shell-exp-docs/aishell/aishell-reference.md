---
title: AIShell command reference
description: Learn about the command-line options and commands available in AIShell.
ms.date: 10/29/2024
---
# AIShell command reference

## Command-line options

```
Description:
  AI for the command line.

Usage:
  aish [<query>] [options]

Arguments:
  <query>  The query term used to get response from AI. []

Options:
  --channel <channel>              A named pipe used to setup communication between aish and the command-line shell.
  --shell-wrapper <shell-wrapper>  Path to the configuration file to wrap AIShell as a different application.
  --version                        Show version information
  -?, -h, --help                   Show help and usage information
```

## Chat commands

By default, `aish` provides a base set of chat commands used to interact with the AI model. To get a
list of commands, use the `/help` command in the chat session.

```
  Name       Description                                      Source
──────────────────────────────────────────────────────────────────────
  /agent     Command for agent management.                    Core
  /cls       Clear the screen.                                Core
  /code      Command to interact with the code generated.     Core
  /dislike   Dislike the last response and send feedback.     Core
  /exit      Exit the interactive session.                    Core
  /help      Show all available commands.                     Core
  /like      Like the last response and send feedback.        Core
  /refresh   Refresh the chat session.                        Core
  /render    Render a markdown file, for diagnosis purpose.   Core
  /retry     Regenerate a new response for the last query.    Core
```

<!-- TO DO
- Add subcommands and switches for each command.
- Add examples for each subcommand.
-->
