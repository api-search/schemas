---
description: ''
layout: schema
name: ContentHistory
properties_list:
- description: ''
  name: latest
  type: boolean
- description: ''
  name: createdDate
  type: string
- description: ''
  name: contributors
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-history-schema.json
slug: atlassian-confluence-content-content-history
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentHistory\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latest\": {\n      \"type\": \"boolean\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\"\n    },\n    \"contributors\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-history-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentHistory
---
