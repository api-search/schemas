---
description: Specifies when and how to create snapshots.
layout: schema
name: Create Rule
properties_list:
- description: The interval between snapshots
  name: Interval
  type: integer
- description: ''
  name: IntervalUnit
  type: string
- description: ''
  name: Times
  type: array
- description: ''
  name: CronExpression
  type: string
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/create-rule-schema.json
slug: create-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/create-rule-schema.json\",\n  \"title\": \"Create Rule\",\n  \"description\": \"Specifies when and how to create snapshots.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The interval between snapshots\"\n    },\n    \"IntervalUnit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HOURS\"\n      ]\n    },\n    \"Times\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"CronExpression\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/create-rule-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Create Rule
---
