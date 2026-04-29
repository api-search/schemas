---
description: A named range.
layout: schema
name: NamedRange
properties_list:
- description: The ID of the named range.
  name: namedRangeId
  type: string
- description: The name of the named range.
  name: name
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-named-range-schema.json
slug: google-sheets-named-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NamedRange\",\n  \"type\": \"object\",\n  \"description\": \"A named range.\",\n  \"properties\": {\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the named range.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the named range.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-named-range-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: NamedRange
---
