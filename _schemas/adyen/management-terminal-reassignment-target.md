---
description: TerminalReassignmentTarget schema from Adyen API
layout: schema
name: TerminalReassignmentTarget
properties_list:
- description: The unique identifier of the company account to which the terminal is reassigned.
  name: companyId
  type: string
- description: Indicates if the terminal is reassigned to the inventory of the merchant account. - If **true**, the terminal is in the inventory of the merchant account and cannot process transactions. - If **false*
  name: inventory
  type: boolean
- description: The unique identifier of the merchant account to which the terminal is reassigned.
  name: merchantId
  type: string
- description: The unique identifier of the store to which the terminal is reassigned.
  name: storeId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-reassignment-target-schema.json
slug: management-terminal-reassignment-target
source_filename: management-terminal-reassignment-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-reassignment-target-schema.json\",\n  \"title\": \"TerminalReassignmentTarget\",\n  \"description\": \"TerminalReassignmentTarget schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account to which the terminal is reassigned.\",\n      \"type\": \"string\"\n    },\n    \"inventory\": {\n      \"description\": \"Indicates if the terminal is reassigned to the inventory of the merchant account.\\n- If **true**, the terminal is in the inventory of the merchant account and cannot process transactions.\\n- If **false**, the terminal is reassigned directly to the merchant account and can process transactions.\",\n      \"type\": \"boolean\"\n    },\n    \"merchantId\": {\n      \"description\": \"\
  The unique identifier of the merchant account to which the terminal is reassigned.\",\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n      \"description\": \"The unique identifier of the store to which the terminal is reassigned.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"inventory\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-reassignment-target-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalReassignmentTarget
---
