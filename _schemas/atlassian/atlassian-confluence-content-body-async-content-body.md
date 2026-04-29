---
description: ''
layout: schema
name: AsyncContentBody
properties_list:
- description: ''
  name: value
  type: string
- description: ''
  name: representation
  type: string
- description: ''
  name: renderTaskId
  type: string
- description: ''
  name: error
  type: string
- description: Rerunning is reserved for when the job is working, but there is a previous run's value in the cache. You may choose to continue polling, or use the cached value.
  name: status
  type: string
- description: ''
  name: embeddedContent
  type: array
- description: ''
  name: mediaToken
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-body-async-content-body-schema.json
slug: atlassian-confluence-content-body-async-content-body
source_filename: atlassian-confluence-content-body-async-content-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AsyncContentBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"representation\": {\n      \"type\": \"string\"\n    },\n    \"renderTaskId\": {\n      \"type\": \"string\"\n    },\n    \"error\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Rerunning is reserved for when the job is working, but there is a previous run's value in the cache. You may choose to continue polling, or use the cached value.\"\n    },\n    \"embeddedContent\": {\n      \"type\": \"array\"\n    },\n    \"mediaToken\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-body-async-content-body-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: AsyncContentBody
---
