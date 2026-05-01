---
description: A CostGuard scan configuration that identifies cost optimization opportunities and waste across cloud resources.
layout: schema
name: Finout CostGuard Scan
properties_list:
- description: The unique identifier of the scan.
  name: id
  type: string
- description: The name of the scan.
  name: name
  type: string
- description: The last time the scan was executed.
  name: lastRunTime
  type: string
- description: The current status of the scan.
  name: status
  type: string
provider_name: Finout
provider_slug: finout
schema_file: json-schema/cost-guard-scan.json
slug: cost-guard-scan
source_filename: cost-guard-scan.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/finout/blob/main/json-schema/cost-guard-scan.json\",\n  \"title\": \"Finout CostGuard Scan\",\n  \"description\": \"A CostGuard scan configuration that identifies cost optimization opportunities and waste across cloud resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the scan.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the scan.\"\n    },\n    \"lastRunTime\": {\n      \"type\": \"string\",\n      \"description\": \"The last time the scan was executed.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the scan.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/finout/refs/heads/main/json-schema/cost-guard-scan.json
tags:
- Budgets
- Costs
- FinOps
title: Finout CostGuard Scan
---
