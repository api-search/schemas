---
description: Represents a Boomi integration process — an automated workflow that moves and transforms data between connected applications. Processes consist of a start shape (trigger), action shapes (steps), and optional decision logic.
layout: schema
name: Boomi Integration Process
properties_list:
- description: Unique component ID of the integration process (UUID format).
  name: id
  type: string
- description: Display name of the integration process.
  name: name
  type: string
- description: Component type. Always 'process' for integration processes.
  name: type
  type: string
- description: ID of the folder containing this process within the component library.
  name: folderId
  type: string
- description: Whether this process has been deleted from the component library.
  name: deleted
  type: boolean
- description: Version identifier of the current saved version of this process.
  name: currentVersion
  type: string
- description: ISO 8601 timestamp when the process was created.
  name: createdDate
  type: string
- description: ISO 8601 timestamp when the process was last modified.
  name: modifiedDate
  type: string
- description: Scheduling configurations for running this process on a time-based trigger.
  name: schedules
  type: array
- description: Active deployments of this process across environments.
  name: deployments
  type: array
provider_name: Boomi
provider_slug: boomi
schema_file: json-schema/boomi-process-schema.json
slug: boomi-process
tags:
- AI Agents
- Automation
- B2B
- Data Integration
- EDI
- Integrations
- Management
- MFT
- Platform
- Workflows
title: Boomi Integration Process
---
