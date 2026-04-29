---
description: A specific action available for a connector
layout: schema
name: ConnectorAction
properties_list:
- description: Unique identifier for the action
  name: actionId
  type: string
- description: Display name of the action
  name: name
  type: string
- description: Description of what the action does
  name: description
  type: string
- description: Parameters accepted by this action
  name: parameters
  type: array
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-connector_action-schema.json
slug: alloy-connectivity-connector_action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-connector_action-schema.json\",\n  \"title\": \"ConnectorAction\",\n  \"type\": \"object\",\n  \"description\": \"A specific action available for a connector\",\n  \"properties\": {\n    \"actionId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the action\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the action\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of what the action does\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"Parameters accepted by this action\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-connector_action-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ConnectorAction
---
