---
description: Terminal schema from Adyen API
layout: schema
name: Terminal
properties_list:
- description: Indicates the account level to which the terminal is assigned, the [assignment status](https://docs.adyen.com/point-of-sale/automating-terminal-management/assign-terminals-api), and where the terminal
  name: assignment
  type: object
- description: Information about bluetooth, cellular, ethernet and wifi connectivity for the terminal.
  name: connectivity
  type: object
- description: The software release currently in use on the terminal.
  name: firmwareVersion
  type: string
- description: The unique identifier of the terminal.
  name: id
  type: string
- description: Date and time of the last activity on the terminal. Not included when the last activity was more than 14 days ago.
  name: lastActivityAt
  type: string
- description: Date and time of the last transaction on the terminal. Not included when the last transaction was more than 14 days ago.
  name: lastTransactionAt
  type: string
- description: The model name of the terminal.
  name: model
  type: string
- description: The serial number of the terminal.
  name: serialNumber
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-schema.json
slug: management-terminal
source_filename: management-terminal-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-schema.json\",\n  \"title\": \"Terminal\",\n  \"description\": \"Terminal schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assignment\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Indicates the account level to which the terminal is assigned, the [assignment status](https://docs.adyen.com/point-of-sale/automating-terminal-management/assign-terminals-api), and where the terminals is in the process of being reassigned to.\",\n      \"$ref\": \"#/components/schemas/TerminalAssignment\"\n    },\n    \"connectivity\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Information about bluetooth, cellular, ethernet and wifi connectivity for the terminal.\",\n      \"$ref\": \"#/components/schemas/TerminalConnectivity\"\n    },\n    \"\
  firmwareVersion\": {\n      \"description\": \"The software release currently in use on the terminal.\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the terminal.\",\n      \"type\": \"string\"\n    },\n    \"lastActivityAt\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Date and time of the last activity on the terminal. Not included when the last activity was more than 14 days ago.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"lastTransactionAt\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"Date and time of the last transaction on the terminal. Not included when the last transaction was more than 14 days ago.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"model\": {\n      \"x-addedInVersion\": \"2\",\n      \"description\": \"The model name of the terminal.\",\n      \"type\": \"string\"\n    },\n    \"serialNumber\": {\n\
  \      \"description\": \"The serial number of the terminal.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: Terminal
---
