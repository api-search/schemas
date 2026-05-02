---
description: Represents a diagnostic setting that configures how platform logs and metrics from Azure resources are routed to destinations such as Log Analytics workspaces, Storage Accounts, and Event Hubs.
layout: schema
name: Azure Monitor Diagnostic Setting
properties_list:
- description: Fully qualified resource ID.
  name: id
  type: string
- description: The name of the resource.
  name: name
  type: string
- description: The type of the resource.
  name: type
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-diagnostic-setting-schema.json
slug: azure-monitor-diagnostic-setting
source_filename: azure-monitor-diagnostic-setting-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/diagnostic-setting.json\",\n  \"title\": \"Azure Monitor Diagnostic Setting\",\n  \"description\": \"Represents a diagnostic setting that configures how platform logs and metrics from Azure resources are routed to destinations such as Log Analytics workspaces, Storage Accounts, and Event Hubs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Fully qualified resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The name of the resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The type of the resource.\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/DiagnosticSettings\"\n    }\n  },\n  \"$defs\": {\n    \"DiagnosticSettings\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"storageAccountId\": {\n          \"type\": \"string\",\n          \"description\": \"The resource ID of the storage account to which you would like to send Diagnostic Logs.\"\n        },\n        \"serviceBusRuleId\": {\n          \"type\": \"string\",\n          \"description\": \"The service bus rule ID of the diagnostic setting. This is here to maintain backwards compatibility.\"\n        },\n        \"eventHubAuthorizationRuleId\": {\n          \"type\": \"string\",\n          \"description\": \"The resource ID of the Event Hub authorization rule.\"\n        },\n        \"eventHubName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the Event Hub. If none is specified, the default Event Hub will be selected.\"\n        },\n        \"metrics\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/MetricSettings\" },\n          \"description\": \"The list of metric\
  \ settings.\"\n        },\n        \"logs\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/LogSettings\" },\n          \"description\": \"The list of logs settings.\"\n        },\n        \"workspaceId\": {\n          \"type\": \"string\",\n          \"description\": \"The full ARM resource ID of the Log Analytics workspace to which you would like to send Diagnostic Logs.\"\n        },\n        \"marketplacePartnerId\": {\n          \"type\": \"string\",\n          \"description\": \"The full ARM resource ID of the Marketplace resource to which you would like to send Diagnostic Logs.\"\n        },\n        \"logAnalyticsDestinationType\": {\n          \"type\": \"string\",\n          \"description\": \"A string indicating whether the export to Log Analytics should use the default destination type or use resource-specific (Dedicated).\"\n        }\n      }\n    },\n    \"MetricSettings\": {\n      \"type\": \"object\",\n      \"required\": [\"enabled\"],\n\
  \      \"properties\": {\n        \"timeGrain\": {\n          \"type\": \"string\",\n          \"description\": \"The timegrain of the metric in ISO 8601 format.\"\n        },\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Name of a Diagnostic Metric category for a resource type.\"\n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"A value indicating whether this category is enabled.\"\n        },\n        \"retentionPolicy\": { \"$ref\": \"#/$defs/RetentionPolicy\" }\n      }\n    },\n    \"LogSettings\": {\n      \"type\": \"object\",\n      \"required\": [\"enabled\"],\n      \"properties\": {\n        \"category\": {\n          \"type\": \"string\",\n          \"description\": \"Name of a Diagnostic Log category for a resource type.\"\n        },\n        \"categoryGroup\": {\n          \"type\": \"string\",\n          \"description\": \"Name of a Diagnostic Log category group for a resource type.\"\
  \n        },\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"A value indicating whether this log is enabled.\"\n        },\n        \"retentionPolicy\": { \"$ref\": \"#/$defs/RetentionPolicy\" }\n      }\n    },\n    \"RetentionPolicy\": {\n      \"type\": \"object\",\n      \"required\": [\"enabled\", \"days\"],\n      \"properties\": {\n        \"enabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"A value indicating whether the retention policy is enabled.\"\n        },\n        \"days\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"description\": \"The number of days for the retention in days. A value of 0 will retain the events indefinitely.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-diagnostic-setting-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Diagnostic Setting
---
