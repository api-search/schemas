---
description: The specification of a BigQuery data source that is connected to a sheet.
layout: schema
name: BigQueryDataSourceSpec
properties_list:
- description: The ID of a BigQuery enabled Google Cloud project with a billing account attached.
  name: projectId
  type: string
- description: A BigQueryQuerySpec.
  name: querySpec
  type: object
- description: A BigQueryTableSpec.
  name: tableSpec
  type: object
provider_name: Google Sheets
provider_slug: google-sheets
schema_file: json-schema/google-sheets-big-query-data-source-spec-schema.json
slug: google-sheets-big-query-data-source-spec
source_filename: google-sheets-big-query-data-source-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BigQueryDataSourceSpec\",\n  \"type\": \"object\",\n  \"description\": \"The specification of a BigQuery data source that is connected to a sheet.\",\n  \"properties\": {\n    \"projectId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of a BigQuery enabled Google Cloud project with a billing account attached.\"\n    },\n    \"querySpec\": {\n      \"type\": \"object\",\n      \"description\": \"A BigQueryQuerySpec.\"\n    },\n    \"tableSpec\": {\n      \"type\": \"object\",\n      \"description\": \"A BigQueryTableSpec.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-sheets/refs/heads/main/json-schema/google-sheets-big-query-data-source-spec-schema.json
tags:
- Google Workspace
- Productivity
- Spreadsheets
title: BigQueryDataSourceSpec
---
