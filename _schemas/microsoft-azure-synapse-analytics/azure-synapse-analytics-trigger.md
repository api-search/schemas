---
description: A trigger resource that orchestrates pipeline execution through schedule-based, tumbling window, or event-based mechanisms.
layout: schema
name: Azure Synapse Analytics Trigger
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: etag
  type: string
- description: ''
  name: properties
  type: object
provider_name: Azure Synapse Analytics
provider_slug: microsoft-azure-synapse-analytics
schema_file: json-schema/azure-synapse-analytics-trigger-schema.json
slug: azure-synapse-analytics-trigger
source_filename: azure-synapse-analytics-trigger-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/azure-synapse-analytics/json-schema/azure-synapse-analytics-trigger-schema.json\",\n  \"title\": \"Azure Synapse Analytics Trigger\",\n  \"description\": \"A trigger resource that orchestrates pipeline execution through schedule-based, tumbling window, or event-based mechanisms.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"etag\": {\n      \"type\": \"string\",\n      \"readOnly\": true\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"required\": [\"type\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"Trigger type.\"\n        },\n        \"description\": {\n    \
  \      \"type\": \"string\"\n        },\n        \"runtimeState\": {\n          \"type\": \"string\",\n          \"readOnly\": true,\n          \"enum\": [\"Started\", \"Stopped\", \"Disabled\"]\n        },\n        \"annotations\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        },\n        \"pipelines\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"pipelineReference\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"referenceName\": {\n                    \"type\": \"string\"\n                  },\n                  \"type\": {\n                    \"type\": \"string\"\n                  }\n                }\n              },\n              \"parameters\": {\n                \"type\": \"object\",\n                \"additionalProperties\": true\n              }\n            }\n\
  \          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-synapse-analytics/refs/heads/main/json-schema/azure-synapse-analytics-trigger-schema.json
tags:
- Analytics
- Apache Spark
- Big Data
- Data Integration
- Data Warehouse
- ETL
- SQL
title: Azure Synapse Analytics Trigger
---
