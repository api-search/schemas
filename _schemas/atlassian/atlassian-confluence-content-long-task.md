---
description: ''
layout: schema
name: LongTask
properties_list:
- description: the ARI for the long task, based on its ID
  name: ari
  type: string
- description: a unique identifier for the long task
  name: id
  type: string
- description: ''
  name: links
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-long-task-schema.json
slug: atlassian-confluence-content-long-task
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LongTask\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ari\": {\n      \"type\": \"string\",\n      \"description\": \"the ARI for the long task, based on its ID\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"a unique identifier for the long task\"\n    },\n    \"links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-long-task-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: LongTask
---
