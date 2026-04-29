---
description: Specifies retention settings for snapshots.
layout: schema
name: Retain Rule
properties_list:
- description: The number of snapshots to retain
  name: Count
  type: integer
- description: ''
  name: Interval
  type: integer
- description: ''
  name: IntervalUnit
  type: string
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/retain-rule-schema.json
slug: retain-rule
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/retain-rule-schema.json\",\n  \"title\": \"Retain Rule\",\n  \"description\": \"Specifies retention settings for snapshots.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Count\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of snapshots to retain\"\n    },\n    \"Interval\": {\n      \"type\": \"integer\"\n    },\n    \"IntervalUnit\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DAYS\",\n        \"WEEKS\",\n        \"MONTHS\",\n        \"YEARS\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/retain-rule-schema.json
tags:
- AWS
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Retain Rule
---
