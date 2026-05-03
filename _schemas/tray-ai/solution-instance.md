---
description: An instance of a published solution created for a specific end user.
layout: schema
name: Tray.ai Solution Instance
properties_list:
- description: Unique solution instance identifier
  name: id
  type: string
- description: Name of the solution instance
  name: name
  type: string
- description: Whether the solution instance is currently enabled
  name: enabled
  type: boolean
- description: Timestamp when the instance was created
  name: created
  type: string
- description: User ID of the instance owner
  name: owner
  type: string
- description: The ID of the solution this instance is based on
  name: solutionId
  type: string
- description: Authentication values configured for this instance
  name: authValues
  type: array
- description: Configuration values set for this instance
  name: configValues
  type: array
- description: Workflows associated with this instance
  name: workflows
  type: object
- description: ''
  name: solutionVersionFlags
  type: object
provider_name: Tray.ai
provider_slug: tray-ai
schema_file: json-schema/solution-instance.json
slug: solution-instance
source_filename: solution-instance.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/solution-instance.json\",\n  \"title\": \"Tray.ai Solution Instance\",\n  \"description\": \"An instance of a published solution created for a specific end user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique solution instance identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the solution instance\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the solution instance is currently enabled\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the instance was created\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"User ID of the\
  \ instance owner\"\n    },\n    \"solutionId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the solution this instance is based on\"\n    },\n    \"authValues\": {\n      \"type\": \"array\",\n      \"description\": \"Authentication values configured for this instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"externalId\": {\n            \"type\": \"string\",\n            \"description\": \"External identifier for the auth slot\"\n          },\n          \"authId\": {\n            \"type\": \"string\",\n            \"description\": \"The authentication ID assigned to this slot\"\n          }\n        }\n      }\n    },\n    \"configValues\": {\n      \"type\": \"array\",\n      \"description\": \"Configuration values set for this instance\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"externalId\": {\n            \"type\": \"string\",\n            \"description\": \"\
  External identifier for the config slot\"\n          },\n          \"value\": {\n            \"type\": \"string\",\n            \"description\": \"The configured value\"\n          }\n        }\n      }\n    },\n    \"workflows\": {\n      \"type\": \"object\",\n      \"description\": \"Workflows associated with this instance\",\n      \"properties\": {\n        \"edges\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"node\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"id\": {\n                    \"type\": \"string\",\n                    \"description\": \"Workflow identifier\"\n                  },\n                  \"triggerUrl\": {\n                    \"type\": \"string\",\n                    \"format\": \"uri\",\n                    \"description\": \"URL to trigger the workflow\"\n                  }\n                }\n         \
  \     }\n            }\n          }\n        }\n      }\n    },\n    \"solutionVersionFlags\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"hasNewerVersion\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether a newer version of the solution is available\"\n        }\n      }\n    }\n  },\n  \"required\": [\"id\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tray-ai/refs/heads/main/json-schema/solution-instance.json
tags:
- Automation
- Integration
- iPaaS
title: Tray.ai Solution Instance
---
