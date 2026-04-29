---
description: TerminalConnectivityCellular schema from Adyen API
layout: schema
name: TerminalConnectivityCellular
properties_list:
- description: The integrated circuit card identifier (ICCID) of the SIM card in the terminal.
  name: iccid
  type: string
- description: On a terminal that supports 3G or 4G connectivity, indicates the status of the SIM card in the terminal.
  name: status
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-connectivity-cellular-schema.json
slug: management-terminal-connectivity-cellular
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-cellular-schema.json\",\n  \"title\": \"TerminalConnectivityCellular\",\n  \"description\": \"TerminalConnectivityCellular schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"iccid\": {\n      \"description\": \"The integrated circuit card identifier (ICCID) of the SIM card in the terminal.\",\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"description\": \"On a terminal that supports 3G or 4G connectivity, indicates the status of the SIM card in the terminal.\",\n      \"enum\": [\n        \"activated\",\n        \"deactivated\",\n        \"deprecated\",\n        \"inventory\",\n        \"readyForActivation\"\n      ],\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-cellular-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalConnectivityCellular
---
