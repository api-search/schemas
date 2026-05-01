---
description: An asset check evaluation result reported to Dagster.
layout: schema
name: AssetCheck
properties_list:
- description: The asset key the check applies to.
  name: asset_key
  type: string
- description: The identifier of the asset check.
  name: check_name
  type: string
- description: True if the check passed, false otherwise.
  name: passed
  type: boolean
- description: Severity level for failed checks.
  name: severity
  type: string
- description: Free-form key/value metadata about the check evaluation.
  name: metadata
  type: object
provider_name: Dagster
provider_slug: dagster
schema_file: json-schema/asset-check.json
slug: asset-check
source_filename: asset-check.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/json-schema/asset-check.json\",\n  \"title\": \"AssetCheck\",\n  \"description\": \"An asset check evaluation result reported to Dagster.\",\n  \"type\": \"object\",\n  \"required\": [\"asset_key\", \"check_name\", \"passed\"],\n  \"properties\": {\n    \"asset_key\": {\n      \"type\": \"string\",\n      \"description\": \"The asset key the check applies to.\"\n    },\n    \"check_name\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the asset check.\"\n    },\n    \"passed\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the check passed, false otherwise.\"\n    },\n    \"severity\": {\n      \"type\": \"string\",\n      \"description\": \"Severity level for failed checks.\",\n      \"enum\": [\"WARN\", \"ERROR\"]\n    },\n    \"metadata\": {\n      \"type\": \"object\",\n\
  \      \"description\": \"Free-form key/value metadata about the check evaluation.\",\n      \"additionalProperties\": true\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dagster/refs/heads/main/json-schema/asset-check.json
tags:
- Data Engineering
- Data Orchestration
- Data Pipelines
- ETL
- Workflows
- Assets
- GraphQL
title: AssetCheck
---
