---
description: ''
layout: schema
name: ContentPropertyUpdate
properties_list:
- description: The value of the content property. This can be empty or a complex object.
  name: value
  type: string
- description: The version number of the property.
  name: version
  type: object
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-content-property-update-schema.json
slug: atlassian-confluence-content-content-property-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContentPropertyUpdate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The value of the content property. This can be empty or a complex object.\"\n    },\n    \"version\": {\n      \"type\": \"object\",\n      \"description\": \"The version number of the property.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-content-property-update-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: ContentPropertyUpdate
---
