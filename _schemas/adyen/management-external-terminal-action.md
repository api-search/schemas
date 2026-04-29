---
description: ExternalTerminalAction schema from Adyen API
layout: schema
name: ExternalTerminalAction
properties_list:
- description: 'The type of terminal action: **InstallAndroidApp**, **UninstallAndroidApp**, **InstallAndroidCertificate**, or **UninstallAndroidCertificate**.'
  name: actionType
  type: string
- description: Technical information about the terminal action.
  name: config
  type: string
- description: The date and time when the action was carried out.
  name: confirmedAt
  type: string
- description: The unique ID of the terminal action.
  name: id
  type: string
- description: The result message for the action.
  name: result
  type: string
- description: The date and time when the action was scheduled to happen.
  name: scheduledAt
  type: string
- description: 'The status of the terminal action: **pending**, **successful**, **failed**, **cancelled**, or **tryLater**.'
  name: status
  type: string
- description: The unique ID of the terminal that the action applies to.
  name: terminalId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-external-terminal-action-schema.json
slug: management-external-terminal-action
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-external-terminal-action-schema.json\",\n  \"title\": \"ExternalTerminalAction\",\n  \"description\": \"ExternalTerminalAction schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"description\": \"The type of terminal action: **InstallAndroidApp**, **UninstallAndroidApp**, **InstallAndroidCertificate**, or **UninstallAndroidCertificate**.\",\n      \"type\": \"string\"\n    },\n    \"config\": {\n      \"description\": \"Technical information about the terminal action.\",\n      \"type\": \"string\"\n    },\n    \"confirmedAt\": {\n      \"description\": \"The date and time when the action was carried out.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"The unique ID of the terminal action.\"\
  ,\n      \"type\": \"string\"\n    },\n    \"result\": {\n      \"description\": \"The result message for the action.\",\n      \"type\": \"string\"\n    },\n    \"scheduledAt\": {\n      \"description\": \"The date and time when the action was scheduled to happen.\",\n      \"format\": \"date-time\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"The status of the terminal action: **pending**, **successful**, **failed**, **cancelled**, or **tryLater**.\",\n      \"type\": \"string\"\n    },\n    \"terminalId\": {\n      \"description\": \"The unique ID of the terminal that the action applies to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-external-terminal-action-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: ExternalTerminalAction
---
