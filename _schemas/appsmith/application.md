---
description: An Appsmith low-code application
layout: schema
name: Application
properties_list:
- description: Unique application identifier
  name: applicationId
  type: string
- description: Application name
  name: name
  type: string
- description: Application description
  name: description
  type: string
- description: Workspace the application belongs to
  name: workspaceId
  type: string
- description: Whether the application is publicly accessible
  name: isPublic
  type: boolean
- description: Application creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
- description: Pages within the application
  name: pages
  type: array
provider_name: Appsmith
provider_slug: appsmith
schema_file: json-schema/application-schema.json
slug: application
tags:
- Low-Code
- Open Source
- Internal Tools
- Workflow Automation
- Developer Tools
title: Application
---
