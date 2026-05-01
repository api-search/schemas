---
description: Specifies the schedule for creating snapshots.
layout: schema
name: Schedule
properties_list:
- description: The name of the schedule
  name: Name
  type: string
- description: ''
  name: CreateRule
  type: object
- description: ''
  name: RetainRule
  type: object
- description: ''
  name: TagsToAdd
  type: array
- description: ''
  name: CopyTags
  type: boolean
provider_name: Amazon Data Lifecycle Manager
provider_slug: amazon-data-lifecycle-manager
schema_file: json-schema/schedule-schema.json
slug: schedule
source_filename: schedule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-data-lifecycle-manager/json-schema/schedule-schema.json\",\n  \"title\": \"Schedule\",\n  \"description\": \"Specifies the schedule for creating snapshots.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the schedule\"\n    },\n    \"CreateRule\": {\n      \"type\": \"object\"\n    },\n    \"RetainRule\": {\n      \"type\": \"object\"\n    },\n    \"TagsToAdd\": {\n      \"type\": \"array\"\n    },\n    \"CopyTags\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-data-lifecycle-manager/refs/heads/main/json-schema/schedule-schema.json
tags:
- Backup
- EBS Snapshots
- Lifecycle Management
- Storage
- Automation
- Compliance
title: Schedule
---
