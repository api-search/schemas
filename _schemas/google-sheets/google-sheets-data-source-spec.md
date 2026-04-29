---
description: This specifies the details of the data source.
layout: schema
name: DataSourceSpec
properties_list:
- description: The parameters of the data source, used when querying the data source.
  name: parameters
  type: array
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-data-source-spec-schema.json
slug: google-sheets-data-source-spec
source_filename: google-sheets-data-source-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DataSourceSpec\",\n  \"type\": \"object\",\n  \"description\": \"This specifies the details of the data source.\",\n  \"properties\": {\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"The parameters of the data source, used when querying the data source.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-data-source-spec-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: DataSourceSpec
---
