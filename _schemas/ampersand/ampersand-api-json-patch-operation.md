---
description: Represents a single JSON Patch operation (RFC 6902). Only supports add, remove, and replace operations for config updates.
layout: schema
name: JSONPatchOperation
properties_list:
- description: 'The operation to perform. - "add": Adds a new field or replaces an existing one at the specified path - "remove": Removes the field at the specified path - "replace": Replaces the value at the specifi'
  name: op
  type: string
- description: JSON Pointer path to the field to operate on (RFC 6901). All paths must start with "/" (e.g., "/schedule", "/selectedFields/phone").
  name: path
  type: string
- description: The value to set for add/replace operations. Not used for remove operations.
  name: value
  type: object
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-json-patch-operation-schema.json
slug: ampersand-api-json-patch-operation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-json-patch-operation-schema.json\",\n  \"title\": \"JSONPatchOperation\",\n  \"description\": \"Represents a single JSON Patch operation (RFC 6902).\\nOnly supports add, remove, and replace operations for config updates.\\n\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"op\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"add\",\n        \"remove\",\n        \"replace\"\n      ],\n      \"description\": \"The operation to perform.\\n- \\\"add\\\": Adds a new field or replaces an existing one at the specified path\\n- \\\"remove\\\": Removes the field at the specified path\\n- \\\"replace\\\": Replaces the value at the specified path\\n\",\n      \"example\": \"replace\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"JSON Pointer path to the\
  \ field to operate on (RFC 6901).\\nAll paths must start with \\\"/\\\" (e.g., \\\"/schedule\\\", \\\"/selectedFields/phone\\\").\\n\",\n      \"example\": \"/schedule\"\n    },\n    \"value\": {\n      \"description\": \"The value to set for add/replace operations.\\nNot used for remove operations.\\n\",\n      \"example\": \"*/10 * * * *\"\n    }\n  },\n  \"required\": [\n    \"op\",\n    \"path\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-json-patch-operation-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: JSONPatchOperation
---
