---
description: Represents an Azure Monitor alert rule resource that defines conditions for triggering alerts and the actions to take when conditions are met.
layout: schema
name: Azure Monitor Alert Rule
properties_list:
- description: Azure resource ID.
  name: id
  type: string
- description: Azure resource name.
  name: name
  type: string
- description: Azure resource type.
  name: type
  type: string
- description: Resource location.
  name: location
  type: string
- description: Resource tags.
  name: tags
  type: object
- description: ''
  name: properties
  type: object
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-alert-rule-schema.json
slug: azure-monitor-alert-rule
source_filename: azure-monitor-alert-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/alert-rule.json\",\n  \"title\": \"Azure Monitor Alert Rule\",\n  \"description\": \"Represents an Azure Monitor alert rule resource that defines conditions for triggering alerts and the actions to take when conditions are met.\",\n  \"type\": \"object\",\n  \"required\": [\"location\", \"properties\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource name.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Azure resource type.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Resource location.\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"\
  additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Resource tags.\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/AlertRule\"\n    }\n  },\n  \"$defs\": {\n    \"AlertRule\": {\n      \"type\": \"object\",\n      \"required\": [\"name\", \"isEnabled\", \"condition\"],\n      \"properties\": {\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the alert rule.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The description of the alert rule that is included in the alert email.\"\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"description\": \"The provisioning state.\"\n        },\n        \"isEnabled\": {\n          \"type\": \"boolean\",\n          \"description\": \"The flag that indicates whether the alert rule is enabled.\"\n        },\n        \"condition\": {\n          \"$ref\": \"#/$defs/RuleCondition\"\
  ,\n          \"description\": \"The condition that results in the alert rule being activated.\"\n        },\n        \"lastUpdatedTime\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\",\n          \"readOnly\": true,\n          \"description\": \"Last time the rule was updated in ISO 8601 format.\"\n        },\n        \"actions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"$ref\": \"#/$defs/RuleAction\"\n          },\n          \"description\": \"The array of actions that are performed when the alert rule becomes active and when an alert condition is resolved.\"\n        }\n      }\n    },\n    \"RuleCondition\": {\n      \"type\": \"object\",\n      \"required\": [\"odata.type\"],\n      \"properties\": {\n        \"odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the type of condition, e.g., ThresholdRuleCondition, LocationThresholdRuleCondition, ManagementEventRuleCondition.\"\n        },\n\
  \        \"dataSource\": {\n          \"$ref\": \"#/$defs/RuleDataSource\"\n        }\n      }\n    },\n    \"RuleDataSource\": {\n      \"type\": \"object\",\n      \"required\": [\"odata.type\"],\n      \"properties\": {\n        \"odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the type of data source, e.g., RuleMetricDataSource, RuleManagementEventDataSource.\"\n        },\n        \"resourceUri\": {\n          \"type\": \"string\",\n          \"description\": \"The resource identifier of the resource the rule monitors.\"\n        },\n        \"legacyResourceId\": {\n          \"type\": \"string\",\n          \"description\": \"The legacy resource identifier.\"\n        },\n        \"resourceLocation\": {\n          \"type\": \"string\",\n          \"description\": \"The location of the resource.\"\n        },\n        \"metricNamespace\": {\n          \"type\": \"string\",\n          \"description\": \"The namespace of the metric.\"\n     \
  \   }\n      }\n    },\n    \"RuleAction\": {\n      \"type\": \"object\",\n      \"required\": [\"odata.type\"],\n      \"properties\": {\n        \"odata.type\": {\n          \"type\": \"string\",\n          \"description\": \"Specifies the type of the action, e.g., RuleEmailAction, RuleWebhookAction.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-alert-rule-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Alert Rule
---
