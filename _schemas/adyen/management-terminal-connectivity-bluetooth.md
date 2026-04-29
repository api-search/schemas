---
description: TerminalConnectivityBluetooth schema from Adyen API
layout: schema
name: TerminalConnectivityBluetooth
properties_list:
- description: The terminal's Bluetooth IP address.
  name: ipAddress
  type: string
- description: The terminal's Bluetooth MAC address.
  name: macAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-connectivity-bluetooth-schema.json
slug: management-terminal-connectivity-bluetooth
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-bluetooth-schema.json\",\n  \"title\": \"TerminalConnectivityBluetooth\",\n  \"description\": \"TerminalConnectivityBluetooth schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAddress\": {\n      \"description\": \"The terminal's Bluetooth IP address.\",\n      \"type\": \"string\"\n    },\n    \"macAddress\": {\n      \"description\": \"The terminal's Bluetooth MAC address.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-bluetooth-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalConnectivityBluetooth
---
