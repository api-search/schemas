---
description: TerminalConnectivityEthernet schema from Adyen API
layout: schema
name: TerminalConnectivityEthernet
properties_list:
- description: The terminal's ethernet IP address.
  name: ipAddress
  type: string
- description: The ethernet link negotiation that the terminal uses.
  name: linkNegotiation
  type: string
- description: The terminal's ethernet MAC address.
  name: macAddress
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-terminal-connectivity-ethernet-schema.json
slug: management-terminal-connectivity-ethernet
source_filename: management-terminal-connectivity-ethernet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-ethernet-schema.json\",\n  \"title\": \"TerminalConnectivityEthernet\",\n  \"description\": \"TerminalConnectivityEthernet schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ipAddress\": {\n      \"description\": \"The terminal's ethernet IP address.\",\n      \"type\": \"string\"\n    },\n    \"linkNegotiation\": {\n      \"description\": \"The ethernet link negotiation that the terminal uses.\",\n      \"type\": \"string\"\n    },\n    \"macAddress\": {\n      \"description\": \"The terminal's ethernet MAC address.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-terminal-connectivity-ethernet-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: TerminalConnectivityEthernet
---
