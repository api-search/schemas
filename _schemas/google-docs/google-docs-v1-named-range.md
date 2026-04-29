---
description: A collection of Ranges that have the same named range ID.
layout: schema
name: NamedRange
properties_list:
- description: The ID of the named range.
  name: namedRangeId
  type: string
- description: The name of the named range.
  name: name
  type: string
- description: The ranges that belong to this named range.
  name: ranges
  type: array
provider_name: Google Docs
provider_slug: google-docs
schema_file: json-schema/google-docs-v1-named-range-schema.json
slug: google-docs-v1-named-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NamedRange\",\n  \"type\": \"object\",\n  \"description\": \"A collection of Ranges that have the same named range ID.\",\n  \"properties\": {\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the named range.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the named range.\"\n    },\n    \"ranges\": {\n      \"type\": \"array\",\n      \"description\": \"The ranges that belong to this named range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-docs/refs/heads/main/json-schema/google-docs-v1-named-range-schema.json
tags:
- Collaboration
- Documents
- Google Workspace
- Productivity
- Word Processing
title: NamedRange
---
