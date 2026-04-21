---
description: Schema representing a bot (automation file) stored in the Automation Anywhere Control Room repository, including its metadata, versioning, workspace context, and repository permissions.
layout: schema
name: Automation Anywhere Bot
properties_list:
- description: Unique numeric identifier of the bot file in the Control Room repository
  name: id
  type: integer
- description: Numeric ID of the parent folder containing this bot in the repository hierarchy
  name: parentId
  type: integer
- description: Display name of the bot file as shown in the Control Room repository browser
  name: name
  type: string
- description: Full repository path from the workspace root (e.g., /Automation/Finance/Invoice Processing)
  name: path
  type: string
- description: Type of the repository object
  name: type
  type: string
- description: File size in bytes
  name: size
  type: integer
- description: Current version number of the bot file
  name: version
  type: integer
- description: Whether this version is labeled as the production version
  name: isProductionVersion
  type: boolean
- description: Workspace this bot belongs to
  name: workspaceType
  type: string
- description: Optional human-readable description of the bot's purpose
  name: description
  type: string
- description: ''
  name: permission
  type: object
- description: List of other bot files this bot depends on during execution
  name: dependencies
  type: array
- description: Optional tags applied to the bot for organization and search
  name: tags
  type: array
- description: Username of the Control Room user who created this bot
  name: createdBy
  type: string
- description: ISO 8601 timestamp when the bot was first created in the repository
  name: createdOn
  type: string
- description: Username of the Control Room user who last modified this bot
  name: updatedBy
  type: string
- description: ISO 8601 timestamp when the bot was last modified
  name: updatedOn
  type: string
provider_name: automation-anywhere
provider_slug: automation-anywhere
schema_file: json-schema/automation-anywhere-bot-schema.json
slug: automation-anywhere-bot
tags: []
title: Automation Anywhere Bot
---
