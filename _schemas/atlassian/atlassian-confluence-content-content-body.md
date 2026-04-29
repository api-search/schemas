---
description: ''
layout: schema
name: ContentBody
properties_list:
- description: ''
  name: value
  type: string
- description: ''
  name: representation
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
schema_file: json-schema/atlassian-confluence-content-content-body-schema.json
slug: atlassian-confluence-content-content-body
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentBody\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\"\n    },\n    \"representation\": {\n      \"type\": \"string\"\n    },\n    \"embeddedContent\": {\n      \"type\": \"array\"\n    },\n    \"mediaToken\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-body-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentBody
---
