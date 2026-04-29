---
description: ''
layout: schema
name: JobHistoryEntry
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: company
  type: string
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: description
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/talent-job-history-entry-schema.json
slug: talent-job-history-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobHistoryEntry\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"company\": {\n      \"type\": \"string\"\n    },\n    \"jobTitle\": {\n      \"type\": \"string\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/talent-job-history-entry-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobHistoryEntry
---
