---
description: Container group log analytics information.
layout: schema
name: LogAnalytics
properties_list:
- description: The log type to be used.
  name: logType
  type: string
- description: Metadata for log analytics.
  name: metadata
  type: object
- description: The workspace id for log analytics
  name: workspaceId
  type: string
- description: The workspace key for log analytics
  name: workspaceKey
  type: string
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-log-analytics-schema.json
slug: azure-container-instances-log-analytics
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: LogAnalytics
---
