---
description: ListExternalTerminalActionsResponse schema from Adyen API
layout: schema
name: ListExternalTerminalActionsResponse
properties_list:
- description: The list of terminal actions.
  name: data
  type: array
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-list-external-terminal-actions-response-schema.json
slug: management-list-external-terminal-actions-response
source_filename: management-list-external-terminal-actions-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-list-external-terminal-actions-response-schema.json\",\n  \"title\": \"ListExternalTerminalActionsResponse\",\n  \"description\": \"ListExternalTerminalActionsResponse schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"description\": \"The list of terminal actions.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ExternalTerminalAction\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-list-external-terminal-actions-response-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ListExternalTerminalActionsResponse
---
