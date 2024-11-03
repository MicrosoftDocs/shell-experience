---
title: AIShell FAQ
description: Get answers to common questions about AIShell.
ms.date: 10/29/2024
ms.topic: faq
---

# Frequently Asked Questions

This page provides help with common questions about AIShell, also known as Project Mercury.

## What is Project Mercury?

**Project Mercury** was the code name for AIShell and is a platform that provides a framework for
developers to build their own AI Agents and assistance providers for an AI Shell. Agents provide the
user experience for the LLM and are deeply connected to PowerShell 7. For more, see the
[AIShell architecture][03].

## What operating systems are supported?

We have tested on macOS and Windows operating systems. **AIShell** may work on linux but we
haven't tested it can't guarantee that all features will work as expected.

## What are the different ways I can use AIShell?

You can use AIShell in two ways:
-   As a standalone application
-   As a split pane experience in PowerShell 7 and Windows Terminal

You can get the split pane experience in other terminals and is based on the capabilities of your
terminal. terminal. For example, Windows Terminal can be split by running the following command:
`wt -w 0 sp`. Refer to the documentation for your terminal application to see if it supports this
feature.

> [!NOTE]
> Not all terminal applications support this feature.

We have made this experience easier when using PowerShell 7 and Windows Terminal. For more information see [Get started with AIShell in PowerShell](./get-started-powershell.md).

## What is the difference between the standalone application and the split pane experience?

The split pane experience with PowerShell 7 has deeper integration with PowerShell and thus can
communicate across the panes for inserting AI generated codes to the working shell and sending
errored commands to the AI pane for assistance. The standalone application is a more generic
experience that can be used with any shell and has no such integration.

## What are AI agents?

An agent is a library that implements the user interface that talks to a specific language
model or other assistance provider. Users can interact with these agents in a conversational manner,
using natural language, to get the desired output or assistance. Currently, these are the supported
agents:

Agent README files:

- [`azure`][01]
- [`openai-gpt`][02]

An assistance provider is an agent that provides user assistance without using a language
model or AI engine.

## How do I create an agent?

To create an agent, you need to implement the `IAgent` interface. You can refer to the page [Create an Ollama Agent][04] for more details on how to create an agent.

## How do I share my agent or find other community built agents?

Currently there is not a centralized repository for sharing and utilizing community built agents. In
the interim, we recommend sharing it on the [discussions page][05] of the Project Mercury
repository.


<!-- link references -->
[01]: agent-azure.md
[02]: agent-openai.md
[03]: developer/agent-architecture.md
[04]: developer/create-ollama-agent.md
[05]: https://github.com/PowerShell/ProjectMercury/discussions/categories/agent-sharing