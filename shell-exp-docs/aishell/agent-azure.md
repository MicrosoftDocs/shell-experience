---
title: Azure agent README
description: Learn how to use the Azure agent in AIShell.
ms.date: 10/29/2024
---
# Copilot in Azure Agent

This agent is designed to connect you to the [**Copilot in Azure**][02] experience directly from
your command line. It provides assistance for Azure CLI commands, Azure PowerShell commands, and
general Azure knowledge. To use this agent, you need to sign into Azure using the `az login` command
from Azure CLI.

> [!IMPORTANT]
> You must use sign into Azure using the Azure CLI command. We're working on supporting the
> `Connect-AzAccount` command from Azure PowerShell.

## Prerequisites

- Windows 11 21H2 or higher
- Windows Terminal v1.19  or higher
- [Azure CLI][01] installed and logged into the allowed tenant

## Sample Questions

- "How do I create a new resource group with Azure CLI?"
- "How can I list out the storage accounts I have in Azure PowerShell?"
- "What is Application Insights?"
- "How to create a web app with Azure CLI?"

## Known issues

Below are some known issues with the Azure agent that we are actively working on addressing:

- The `Connect-AzAccount` command for authentication from Azure PowerShell is not supported. You must use the `az login`
  command from Azure CLI to sign in.

## Telemetry

The **Copilot in Azure** agent captures minor telemetry to help us improve the product experience.
This data collection is limited in scope and only captures detailed telemetry when you consent to
sharing your chat history. We will only capture your chat history when you use a `/like` or
`/dislike` command and consent to sharing your chat history.

During usage, the agent will capture the following information:
- The `/` command that you used
- The count of number of questions asked
- The type of operating system used
- Any exceptions encountered during usage
- Details provided when using `/like` or `/dislike` commands

You can disable this telemetry from being captured by modifying the `telemetry` property in the
configuration file. See the details below.

## Agent Configuration

There are some minor configuration settings that can be set for the Azure agent. You can view and
edit the JSON config file by running `/agent config` while using the Copilot in Azure Agent. The
available settings are:

```json
{
  "logging": true,
  "telemetry": true
}
```
### Logging
When logging is enabled, logs will be saved in the `~\.aish\agent-config\azure` directory. If you
change the setting to be false then no logging will take place.

### Telemetry
Turning the telemetry property to false will disable all telemetry for the agent. All telemetry
captured by default does not contain any personal identifiable information and only captures product
usage data to help us improve the product experience. See the above for additional details.

<!-- link references -->
[01]: /cli/azure/install-azure-cli
[02]: https://azure.microsoft.com/products/copilot
