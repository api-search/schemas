---
description: The properties of a list which describe the look and feel of bullets.
layout: schema
name: ListProperties
properties_list:
- description: Describes the properties of the bullets at the associated level. A list has at most 9 levels of nesting.
  name: nestingLevels
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-list-properties-schema.json
slug: google-docs-v1-list-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListProperties\",\n  \"type\": \"object\",\n  \"description\": \"The properties of a list which describe the look and feel of bullets.\",\n  \"properties\": {\n    \"nestingLevels\": {\n      \"type\": \"array\",\n      \"description\": \"Describes the properties of the bullets at the associated level. A list has at most 9 levels of nesting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-list-properties-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: ListProperties
---
