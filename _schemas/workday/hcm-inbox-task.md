---
description: ''
layout: schema
name: InboxTask
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: assigned
  type: string
- description: ''
  name: due
  type: string
- description: ''
  name: overdue
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-inbox-task-schema.json
slug: hcm-inbox-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InboxTask\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"assigned\": {\n      \"type\": \"string\"\n    },\n    \"due\": {\n      \"type\": \"string\"\n    },\n    \"overdue\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-inbox-task-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: InboxTask
---
