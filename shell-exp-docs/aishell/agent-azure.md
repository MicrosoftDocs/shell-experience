---
title: Azure agent README
description: Learn how to use the Azure agent in AIShell.
ms.date: 10/29/2024
---
# Copilot in Azure Agent

This agent is designed to connect you to the [**Copilot in Azure**][02] experience directly from
your command line. It provides assistance for Azure CLI commands, Azure PowerShell commands and
general Azure knowledge. To use this agent, you need to sign into Azure using the `az login` command
from Azure CLI.

> [!NOTE] Currently, you can only use this tool using the login command from Azure CLI. We are
> working on supporting the equivalent login command from Azure PowerShell.

## Prerequisites

- Windows 11 21H2 or higher
- Windows Terminal v1.19  or higher
- [Azure CLI][01] installed and logged into the allowed tenant

## Sample Questions

- "How do I create a new resource group with Azure CLI?"
- "How can I list out the storage accounts I have in Azure PowerShell?"
- "What is Application Insights?"
- "How to create a web app with Azure CLI?"

<!-- TO DO
- Is there any configuration required?
-->

<!-- link references -->
[01]: /cli/azure/install-azure-cli
[02]: https://azure.microsoft.com/products/copilot
