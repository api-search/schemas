---
description: TerminalConnectivity schema from Adyen API
layout: schema
name: TerminalConnectivity
properties_list:
- description: ''
  name: bluetooth
  type: object
- description: ''
  name: cellular
  type: object
- description: ''
  name: ethernet
  type: object
- description: ''
  name: wifi
  type: object
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-connectivity-schema.json
slug: management-terminal-connectivity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-schema.json\",\n  \"title\": \"TerminalConnectivity\",\n  \"description\": \"TerminalConnectivity schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"bluetooth\": {\n      \"$ref\": \"#/components/schemas/TerminalConnectivityBluetooth\"\n    },\n    \"cellular\": {\n      \"$ref\": \"#/components/schemas/TerminalConnectivityCellular\"\n    },\n    \"ethernet\": {\n      \"$ref\": \"#/components/schemas/TerminalConnectivityEthernet\"\n    },\n    \"wifi\": {\n      \"$ref\": \"#/components/schemas/TerminalConnectivityWifi\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalConnectivity
---
