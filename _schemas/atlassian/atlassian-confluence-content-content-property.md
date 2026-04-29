---
description: ''
layout: schema
name: ContentProperty
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: key
  type: string
- description: The value of the content property. This can be empty or a complex object.
  name: value
  type: string
- description: ''
  name: version
  type: object
- description: ''
  name: _expandable
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-property-schema.json
slug: atlassian-confluence-content-content-property
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentProperty\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the content property. This can be empty or a complex object.\"\n    },\n    \"version\": {\n      \"type\": \"object\"\n    },\n    \"_expandable\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-property-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentProperty
---
