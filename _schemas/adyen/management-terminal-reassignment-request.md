---
description: TerminalReassignmentRequest schema from Adyen API
layout: schema
name: TerminalReassignmentRequest
properties_list:
- description: The unique identifier of the company account to which the terminal is reassigned.
  name: companyId
  type: string
- description: 'Must be specified when reassigning terminals to a merchant account: - If set to **true**, reassigns terminals to the inventory of the merchant account and the terminals cannot process transactions. - '
  name: inventory
  type: boolean
- description: The unique identifier of the merchant account to which the terminal is reassigned. When reassigning terminals to a merchant account, you must specify the `inventory` field.
  name: merchantId
  type: string
- description: The unique identifier of the store to which the terminal is reassigned.
  name: storeId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-reassignment-request-schema.json
slug: management-terminal-reassignment-request
source_filename: management-terminal-reassignment-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-reassignment-request-schema.json\",\n  \"title\": \"TerminalReassignmentRequest\",\n  \"description\": \"TerminalReassignmentRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account to which the terminal is reassigned.\",\n      \"type\": \"string\"\n    },\n    \"inventory\": {\n      \"description\": \"Must be specified when reassigning terminals to a merchant account:\\n\\n- If set to **true**, reassigns terminals to the inventory of the merchant account and the terminals cannot process transactions.\\n\\n- If set to **false**, reassigns terminals directly to the merchant account and the terminals can process transactions.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantId\"\
  : {\n      \"description\": \"The unique identifier of the merchant account to which the terminal is reassigned. When reassigning terminals to a merchant account, you must specify the `inventory` field.\",\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n      \"description\": \"The unique identifier of the store to which the terminal is reassigned.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-reassignment-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalReassignmentRequest
---
