---
description: ''
layout: schema
name: LabelCreate
properties_list:
- description: The prefix for the label. `global`, `my` `team`, etc.
  name: prefix
  type: string
- description: The name of the label, which will be shown in the UI.
  name: name
  type: string
provider_name: Atlassian
provider_slug: atlassian
schema_file: json-schema/atlassian-confluence-content-label-create-schema.json
slug: atlassian-confluence-content-label-create
source_filename: atlassian-confluence-content-label-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LabelCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"prefix\": {\n      \"type\": \"string\",\n      \"description\": \"The prefix for the label. `global`, `my` `team`, etc.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the label, which will be shown in the UI.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/atlassian/refs/heads/main/json-schema/atlassian-confluence-content-label-create-schema.json
tags:
- Code
- Collaboration
- Platform
- Productivity
- Software Development
title: LabelCreate
---
