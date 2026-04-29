---
description: TerminalAssignment schema from Adyen API
layout: schema
name: TerminalAssignment
properties_list:
- description: The unique identifier of the company account to which terminal is assigned.
  name: companyId
  type: string
- description: The unique identifier of the merchant account to which terminal is assigned.
  name: merchantId
  type: string
- description: Indicates where the terminal is in the process of being reassigned to.
  name: reassignmentTarget
  type: object
- description: 'The status of the reassignment. Possible values: * `reassignmentInProgress`: the terminal was boarded and is now scheduled to remove the configuration. Wait for the terminal to synchronize with the Ad'
  name: status
  type: string
- description: The unique identifier of the store to which terminal is assigned.
  name: storeId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-assignment-schema.json
slug: management-terminal-assignment
source_filename: management-terminal-assignment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-assignment-schema.json\",\n  \"title\": \"TerminalAssignment\",\n  \"description\": \"TerminalAssignment schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"description\": \"The unique identifier of the company account to which terminal is assigned.\",\n      \"type\": \"string\"\n    },\n    \"merchantId\": {\n      \"description\": \"The unique identifier of the merchant account to which terminal is assigned.\",\n      \"type\": \"string\"\n    },\n    \"reassignmentTarget\": {\n      \"description\": \"Indicates where the terminal is in the process of being reassigned to.\",\n      \"$ref\": \"#/components/schemas/TerminalReassignmentTarget\"\n    },\n    \"status\": {\n      \"description\": \"The status of the reassignment. Possible values:\
  \ \\n * `reassignmentInProgress`: the terminal was boarded and is now scheduled to remove the configuration. Wait for the terminal to synchronize with the Adyen platform.\\n * `deployed`: the terminal is deployed and reassigned. \\n * `inventory`: the terminal is in inventory and cannot process transactions. \\n * `boarded`: the terminal is boarded to a store, or a merchant account representing a store, and can process transactions. \\n\",\n      \"enum\": [\n        \"boarded\",\n        \"deployed\",\n        \"inventory\",\n        \"reassignmentInProgress\"\n      ],\n      \"type\": \"string\"\n    },\n    \"storeId\": {\n      \"description\": \"The unique identifier of the store to which terminal is assigned.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"companyId\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-assignment-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalAssignment
---
