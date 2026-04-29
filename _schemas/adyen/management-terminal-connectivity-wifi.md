---
description: TerminalConnectivityWifi schema from Adyen API
layout: schema
name: TerminalConnectivityWifi
properties_list:
- description: The terminal's IP address in the Wi-Fi network.
  name: ipAddress
  type: string
- description: The terminal's MAC address in the Wi-Fi network.
  name: macAddress
  type: string
- description: The SSID of the Wi-Fi network that the terminal is connected to.
  name: ssid
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-connectivity-wifi-schema.json
slug: management-terminal-connectivity-wifi
source_filename: management-terminal-connectivity-wifi-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-wifi-schema.json\",\n  \"title\": \"TerminalConnectivityWifi\",\n  \"description\": \"TerminalConnectivityWifi schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAddress\": {\n      \"description\": \"The terminal's IP address in the Wi-Fi network.\",\n      \"type\": \"string\"\n    },\n    \"macAddress\": {\n      \"description\": \"The terminal's MAC address in the Wi-Fi network.\",\n      \"type\": \"string\"\n    },\n    \"ssid\": {\n      \"description\": \"The SSID of the Wi-Fi network that the terminal is connected to.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-wifi-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalConnectivityWifi
---
