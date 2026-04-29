---
description: CommitRequest schema from Avalara API
layout: schema
name: CommitRequest
properties_list:
- description: Document code to commit
  name: doc
  type: string
- description: Commit flag (true to commit)
  name: cmmt
  type: boolean
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/communications-commit-request-schema.json
slug: communications-commit-request
source_filename: communications-commit-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-commit-request-schema.json\",\n  \"title\": \"CommitRequest\",\n  \"description\": \"CommitRequest schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"doc\": {\n      \"type\": \"string\",\n      \"description\": \"Document code to commit\"\n    },\n    \"cmmt\": {\n      \"type\": \"boolean\",\n      \"description\": \"Commit flag (true to commit)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/communications-commit-request-schema.json
tags:
- Taxes
title: CommitRequest
---
