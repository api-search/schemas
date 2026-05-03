---
description: A published solution (integration) available on the Tray.ai platform.
layout: schema
name: Tray.ai Solution
properties_list:
- description: Unique solution identifier
  name: id
  type: string
- description: Title of the solution
  name: title
  type: string
- description: Description of the solution
  name: description
  type: string
- description: Tags associated with the solution
  name: tags
  type: array
- description: Configuration slots that must be filled when creating an instance
  name: configSlots
  type: array
- description: Authentication slots that must be filled when creating an instance
  name: authSlots
  type: array
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/solution.json
slug: solution
source_filename: solution.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/solution.json\",\n  \"title\": \"Tray.ai Solution\",\n  \"description\": \"A published solution (integration) available on the Tray.ai platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique solution identifier\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the solution\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the solution\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags associated with the solution\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"configSlots\": {\n      \"type\": \"array\",\n      \"description\": \"Configuration slots that must be filled when\
  \ creating an instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"externalId\": {\n            \"type\": \"string\",\n            \"description\": \"External identifier for the config slot\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"description\": \"Display name for the config slot\"\n          },\n          \"defaultValue\": {\n            \"type\": \"string\",\n            \"description\": \"Default value for the config slot\"\n          }\n        }\n      }\n    },\n    \"authSlots\": {\n      \"type\": \"array\",\n      \"description\": \"Authentication slots that must be filled when creating an instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"externalId\": {\n            \"type\": \"string\",\n            \"description\": \"External identifier for the auth slot\"\n          },\n          \"title\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"Display name for the auth slot\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/solution.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Solution
---
