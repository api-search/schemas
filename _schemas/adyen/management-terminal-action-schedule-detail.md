---
description: TerminalActionScheduleDetail schema from Adyen API
layout: schema
name: TerminalActionScheduleDetail
properties_list:
- description: The ID of the action on the specified terminal.
  name: id
  type: string
- description: The unique ID of the terminal that the action applies to.
  name: terminalId
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-action-schedule-detail-schema.json
slug: management-terminal-action-schedule-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-action-schedule-detail-schema.json\",\n  \"title\": \"TerminalActionScheduleDetail\",\n  \"description\": \"TerminalActionScheduleDetail schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The ID of the action on the specified terminal.\",\n      \"type\": \"string\"\n    },\n    \"terminalId\": {\n      \"description\": \"The unique ID of the terminal that the action applies to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-action-schedule-detail-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalActionScheduleDetail
---
