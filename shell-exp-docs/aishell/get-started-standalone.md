---
description: This article explains how to install and configure AIShell, and get started chatting with an AI assistant.
ms.date: 10/29/2024
title: Get started with AIShell
---
# Get started with AIShell

AIShell was created to help command line users find the right commands to use, recover from errors,
and better understand the commands and the output they produce. Follow along and walk through some
examples to get started with AIShell.

## Starting AIShell

Run the `aish` command in the shell of your choice. AIShell starts in a new terminal window and
prompts you to choose an agent.

## Using AIShell

Now that you have selected an agent, you can begin chatting with it. The installed Azure OpenAI
agent is configured to be a PowerShell expert. This means we've modified the AI system prompt
to say it should act like a PowerShell expert. It's not trained on any specific PowerShell code or
documentation. In the final version, you must configure the agent with your endpoint, API keys,
and system prompt before using it. For this walkthrough, we've performed these steps for you.

The Azure agent is designed to bring the Copilot in Azure experience directly to your command line.
It provides assistance for Azure CLI and Azure PowerShell commands. To use this agent, you need to
sign into Azure using the `az login` or `Connect-AzAccount` commands.

## Use AIShell to interact with the agents

Use these sample queries with each agent.

Azure OpenAI Agent

- "How do I create a text file named helloworld in PowerShell?"
- "What is the difference between a switch and a parameter in PowerShell?"
- How do I get the top 10 most CPU intensive processes on my computer?

Azure Agent

- "How do I create a new resource group with Azure CLI?"
- "How can I list out the storage accounts I have in Azure PowerShell?"
- "What is Application Insights?"
- "How to create a web app with Azure CLI?"

### Switching Agents

You can switch between agents using the `@<agentName>` syntax in your chat messages. For example,

![An animation showing switching between two agents with the @ sign](/docs/media/SwitchingAgents.gif)

You can also use a chat command to switch agents. For example, to switch to the `openai-gpt` agent,
use `/agent use openai-gpt`.

### Chat commands

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

### Key bindings for commands

AIShell has key bindings for the `/code` command. They key bindings are currently hard-coded, but
custom key bindings will be supported in a future release.

|                  Key binding                  |     Command      |                     Description                     |
| --------------------------------------------- | ---------------- | --------------------------------------------------- |
| <kbd>Ctrl+d</kbd><kbd>Ctrl</kbd>+<kbd>c</kbd> | `/code copy`     | Copy _all_ the generated code snippets to clipboard |
| <kbd>Ctrl</kbd>+<kbd>\<n\></kbd>              | `/code copy <n>` | Copy the _n-th_ generated code snippet to clipboard |
