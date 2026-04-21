---
description: Schema representing a bot deployment request and response in the Automation Anywhere Control Room, including deployment configuration, target device specification, input variables, and the resulting deployment identifier.
layout: schema
name: Automation Anywhere Bot Deployment
properties_list:
- description: Unique UUID identifier assigned to this deployment instance by the Control Room upon successful dispatch
  name: deploymentId
  type: string
- description: Numeric file ID of the bot to deploy, referencing the bot's ID in the repository
  name: botId
  type: integer
- description: Optional human-readable label for this automation instance as displayed in activity logs and dashboards
  name: automationName
  type: string
- description: Optional description of this specific deployment for tracking and audit purposes
  name: description
  type: string
- description: Optional label tag for identifying this deployment instance
  name: botLabel
  type: string
- description: Whether to run the bot with elevated system privileges on the Bot Runner device
  name: runElevated
  type: boolean
- description: Whether to suppress the Bot Agent user interface on the runner device during execution
  name: hideBotAgentUi
  type: boolean
- description: Priority level for this automation in the dispatch queue relative to other pending deployments
  name: automationPriority
  type: string
- description: ''
  name: callbackInfo
  type: object
- description: Runtime input variables to pass to the bot at execution time. Keys are variable names as defined in the bot; values are typed variable objects.
  name: botInput
  type: object
- description: ''
  name: unattendedRequest
  type: object
- description: ''
  name: attendedRequest
  type: object
- description: ''
  name: headlessRequest
  type: object
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-deployment-schema.json
slug: automation-anywhere-deployment
tags: []
title: Automation Anywhere Bot Deployment
---
