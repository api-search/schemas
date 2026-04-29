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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-log-analytics-schema.json\",\n  \"title\": \"LogAnalytics\",\n  \"description\": \"Container group log analytics information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logType\": {\n      \"description\": \"The log type to be used.\",\n      \"enum\": [\n        \"ContainerInsights\",\n        \"ContainerInstanceLogs\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"LogAnalyticsLogType\"\n      }\n    },\n    \"metadata\": {\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Metadata for log analytics.\",\n      \"type\": \"object\"\n    },\n    \"workspaceId\": {\n      \"description\": \"The workspace id for log analytics\",\n      \"\
  type\": \"string\"\n    },\n    \"workspaceKey\": {\n      \"description\": \"The workspace key for log analytics\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"workspaceId\",\n    \"workspaceKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-instances/refs/heads/main/json-schema/azure-container-instances-log-analytics-schema.json
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: LogAnalytics
---
