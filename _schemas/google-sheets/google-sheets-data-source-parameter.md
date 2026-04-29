---
description: A parameter in a data source's query.
layout: schema
name: DataSourceParameter
properties_list:
- description: Named parameter.
  name: name
  type: string
- description: ID of a NamedRange.
  name: namedRangeId
  type: string
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-parameter-schema.json
slug: google-sheets-data-source-parameter
source_filename: google-sheets-data-source-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceParameter\",\n  \"type\": \"object\",\n  \"description\": \"A parameter in a data source's query.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Named parameter.\"\n    },\n    \"namedRangeId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of a NamedRange.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-parameter-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceParameter
---
