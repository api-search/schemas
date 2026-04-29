---
description: Result of a connector action execution
layout: schema
name: ActionResult
properties_list:
- description: Whether the action executed successfully
  name: success
  type: boolean
- description: Action result data
  name: data
  type: object
provider_name: Alloy Automation
provider_slug: alloy-automation
schema_file: json-schema/alloy-connectivity-action_result-schema.json
slug: alloy-connectivity-action_result
source_filename: alloy-connectivity-action_result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.runalloy.com/schemas/alloy-connectivity-action_result-schema.json\",\n  \"title\": \"ActionResult\",\n  \"type\": \"object\",\n  \"description\": \"Result of a connector action execution\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the action executed successfully\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Action result data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/json-schema/alloy-connectivity-action_result-schema.json
tags:
- Automation
- Embedded Integrations
- Integrations
- iPaaS
- Unified API
- Workflows
title: ActionResult
---
