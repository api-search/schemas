---
description: Base object for all content types.
layout: schema
name: Content
properties_list:
- description: ''
  name: id
  type: string
- description: Can be "page", "blogpost", "attachment" or "content"
  name: type
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: title
  type: string
- description: ''
  name: ancestors
  type: array
- description: ''
  name: operations
  type: array
- description: ''
  name: body
  type: object
- description: ''
  name: restrictions
  type: object
- description: ''
  name: macroRenderedOutput
  type: object
- description: ''
  name: extensions
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-schema.json
slug: atlassian-confluence-content-content
source_filename: atlassian-confluence-content-content-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Content\",\n  \"type\": \"object\",\n  \"description\": \"Base object for all content types.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Can be \\\"page\\\", \\\"blogpost\\\", \\\"attachment\\\" or \\\"content\\\"\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"ancestors\": {\n      \"type\": \"array\"\n    },\n    \"operations\": {\n      \"type\": \"array\"\n    },\n    \"body\": {\n      \"type\": \"object\"\n    },\n    \"restrictions\": {\n      \"type\": \"object\"\n    },\n    \"macroRenderedOutput\": {\n      \"type\": \"object\"\n    },\n    \"extensions\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: Content
---
