---
description: Request body for executing a connector action
layout: schema
name: ExecuteActionRequest
properties_list:
- description: Identifier of the user executing the action
  name: userId
  type: string
- description: Credential identifier to use for authentication
  name: credentialId
  type: string
- description: Action-specific parameters
  name: parameters
  type: object
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-execute_action_request-schema.json
slug: alloy-connectivity-execute_action_request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-execute_action_request-schema.json\",\n  \"title\": \"ExecuteActionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for executing a connector action\",\n  \"properties\": {\n    \"userId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the user executing the action\"\n    },\n    \"credentialId\": {\n      \"type\": \"string\",\n      \"description\": \"Credential identifier to use for authentication\"\n    },\n    \"parameters\": {\n      \"type\": \"object\",\n      \"description\": \"Action-specific parameters\"\n    }\n  },\n  \"required\": [\n    \"userId\",\n    \"credentialId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-execute_action_request-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ExecuteActionRequest
---
