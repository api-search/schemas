---
description: ''
layout: schema
name: ContentPropertyCreate
properties_list:
- description: The key of the new property.
  name: key
  type: string
- description: The value of the content property. This can be empty or a complex object.
  name: value
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-property-create-schema.json
slug: atlassian-confluence-content-content-property-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentPropertyCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The key of the new property.\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the content property. This can be empty or a complex object.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-property-create-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentPropertyCreate
---
