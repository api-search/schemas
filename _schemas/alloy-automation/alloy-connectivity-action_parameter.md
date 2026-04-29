---
description: A parameter definition for a connector action
layout: schema
name: ActionParameter
properties_list:
- description: Parameter name
  name: name
  type: string
- description: Parameter data type
  name: type
  type: string
- description: Whether the parameter is required
  name: required
  type: boolean
- description: Description of the parameter
  name: description
  type: string
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-action_parameter-schema.json
slug: alloy-connectivity-action_parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-action_parameter-schema.json\",\n  \"title\": \"ActionParameter\",\n  \"type\": \"object\",\n  \"description\": \"A parameter definition for a connector action\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter data type\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the parameter is required\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the parameter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-action_parameter-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ActionParameter
---
