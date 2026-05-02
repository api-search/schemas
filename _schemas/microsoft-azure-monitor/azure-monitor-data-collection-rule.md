---
description: Represents an Azure Monitor data collection rule that defines data sources, transformations, and destinations for collecting monitoring data.
layout: schema
name: Azure Monitor Data Collection Rule
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
- description: The geo-location where the resource lives.
  name: location
  type: string
- description: ''
  name: tags
  type: object
- description: The kind of the resource.
  name: kind
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Monitor
provider_slug: microsoft-azure-monitor
schema_file: json-schema/azure-monitor-data-collection-rule-schema.json
slug: azure-monitor-data-collection-rule
source_filename: azure-monitor-data-collection-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.azure.com/monitor/data-collection-rule.json\",\n  \"title\": \"Azure Monitor Data Collection Rule\",\n  \"description\": \"Represents an Azure Monitor data collection rule that defines data sources, transformations, and destinations for collecting monitoring data.\",\n  \"type\": \"object\",\n  \"required\": [\"location\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"Fully qualified resource ID.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The name of the resource.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true,\n      \"description\": \"The type of the resource.\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"The geo-location where the resource lives.\"\n    },\n    \"tags\"\
  : {\n      \"type\": \"object\",\n      \"additionalProperties\": { \"type\": \"string\" }\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"enum\": [\"Linux\", \"Windows\"],\n      \"description\": \"The kind of the resource.\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/$defs/DataCollectionRule\"\n    }\n  },\n  \"$defs\": {\n    \"DataCollectionRule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the data collection rule.\"\n        },\n        \"immutableId\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"description\": \"The immutable ID of this data collection rule.\"\n        },\n        \"dataCollectionEndpointId\": {\n          \"type\": \"string\",\n          \"description\": \"The resource ID of the data collection endpoint.\"\n        },\n        \"streamDeclarations\": {\n          \"type\": \"object\",\n\
  \          \"additionalProperties\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"columns\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"name\": { \"type\": \"string\" },\n                    \"type\": { \"type\": \"string\", \"enum\": [\"string\", \"int\", \"long\", \"real\", \"boolean\", \"datetime\", \"dynamic\"] }\n                  }\n                }\n              }\n            }\n          },\n          \"description\": \"Declaration of custom streams used in this rule.\"\n        },\n        \"dataSources\": {\n          \"$ref\": \"#/$defs/DataSources\"\n        },\n        \"destinations\": {\n          \"$ref\": \"#/$defs/Destinations\"\n        },\n        \"dataFlows\": {\n          \"type\": \"array\",\n          \"items\": { \"$ref\": \"#/$defs/DataFlow\" },\n          \"description\": \"The specification\
  \ of data flows.\"\n        },\n        \"provisioningState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\"Creating\", \"Updating\", \"Deleting\", \"Succeeded\", \"Canceled\", \"Failed\"]\n        }\n      }\n    },\n    \"DataSources\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"performanceCounters\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"streams\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"samplingFrequencyInSeconds\": { \"type\": \"integer\" },\n              \"counterSpecifiers\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n            }\n          }\n        },\n        \"windowsEventLogs\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\"\
  : {\n              \"name\": { \"type\": \"string\" },\n              \"streams\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"xPathQueries\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n            }\n          }\n        },\n        \"syslog\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n              \"streams\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"facilityNames\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"logLevels\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n            }\n          }\n        },\n        \"extensions\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"name\": { \"type\": \"string\" },\n      \
  \        \"streams\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n              \"extensionName\": { \"type\": \"string\" },\n              \"extensionSettings\": { \"type\": \"object\", \"additionalProperties\": true },\n              \"inputDataSources\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } }\n            }\n          }\n        }\n      }\n    },\n    \"Destinations\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"logAnalytics\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"workspaceResourceId\": { \"type\": \"string\" },\n              \"workspaceId\": { \"type\": \"string\", \"readOnly\": true },\n              \"name\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"azureMonitorMetrics\": {\n          \"type\": \"object\",\n          \"properties\": { \"name\": { \"type\": \"string\" } }\n     \
  \   },\n        \"eventHubs\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"eventHubResourceId\": { \"type\": \"string\" },\n              \"name\": { \"type\": \"string\" }\n            }\n          }\n        },\n        \"storageBlobsDirect\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"storageAccountResourceId\": { \"type\": \"string\" },\n              \"containerName\": { \"type\": \"string\" },\n              \"name\": { \"type\": \"string\" }\n            }\n          }\n        }\n      }\n    },\n    \"DataFlow\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"streams\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"destinations\": { \"type\": \"array\", \"items\": { \"type\": \"string\" } },\n        \"transformKql\": { \"type\": \"string\"\
  , \"description\": \"The KQL query to transform stream data.\" },\n        \"outputStream\": { \"type\": \"string\" },\n        \"builtInTransform\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-monitor/refs/heads/main/json-schema/azure-monitor-data-collection-rule-schema.json
tags:
- Application Insights
- Cloud
- Logs
- Metrics
- Monitoring
- Observability
title: Azure Monitor Data Collection Rule
---
