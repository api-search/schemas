---
description: An issue detected in the QueryGrid environment.
layout: schema
name: Issue
properties_list:
- description: Unique issue identifier.
  name: id
  type: string
- description: Issue severity level.
  name: severity
  type: string
- description: Issue description message.
  name: message
  type: string
- description: Source component of the issue.
  name: source
  type: string
- description: Time when the issue was detected.
  name: timestamp
  type: string
provider_name: Teradata
provider_slug: teradata
schema_file: json-schema/querygrid-manager-api-issue-schema.json
slug: querygrid-manager-api-issue
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-issue-schema.json\",\n  \"title\": \"Issue\",\n  \"description\": \"An issue detected in the QueryGrid environment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique issue identifier.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Issue severity level.\",\n      \"enum\": [\"info\", \"warning\", \"error\", \"critical\"]\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Issue description message.\"\n    },\n    \"source\": {\n      \"type\": \"string\",\n      \"description\": \"Source component of the issue.\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Time when the issue\
  \ was detected.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/teradata/refs/heads/main/json-schema/querygrid-manager-api-issue-schema.json
tags:
- Analytics
- Cloud
- Data Management
- Data Warehousing
- Database
- Enterprise
- Machine Learning
- SQL
title: Issue
---
