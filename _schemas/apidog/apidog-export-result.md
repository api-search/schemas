---
description: The result returned by the Apidog API after an export operation, containing the exported API specification data.
layout: schema
name: Apidog Export Result
properties_list:
- description: Whether the export operation completed successfully.
  name: success
  type: boolean
- description: The exported API specification data as a string in the requested format (JSON or YAML).
  name: data
  type: string
provider_name: Apidog
provider_slug: apidog
schema_file: json-schema/apidog-export-result-schema.json
slug: apidog-export-result
source_filename: apidog-export-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-export-result-schema.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Apidog Export Result\",\n  \"description\": \"The result returned by the Apidog API after an export operation, containing the exported API specification data.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"success\"\n  ],\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the export operation completed successfully.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"The exported API specification data as a string in the requested format (JSON or YAML).\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apidog/refs/heads/main/json-schema/apidog-export-result-schema.json
tags:
- API Design
- API Lifecycle
- API Testing
- Collaboration
- Design-First
- Documentation
- Mocking
- Platform
title: Apidog Export Result
---
