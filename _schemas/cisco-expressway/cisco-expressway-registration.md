---
description: Schema for a device registration on Cisco Expressway. Represents an endpoint or device currently registered with the Expressway using SIP or H.323 protocols, including contact address, registration time, and subzone assignment.
layout: schema
name: Cisco Expressway Registration
properties_list:
- description: Registered alias of the device, such as a SIP URI or H.323 alias
  name: Alias
  type: string
- description: Registration protocol type
  name: Type
  type: string
- description: Network contact address of the device, including IP address and port
  name: ContactAddress
  type: string
- description: ISO 8601 timestamp when the device registered
  name: RegisteredAt
  type: string
- description: ISO 8601 timestamp when the registration expires and must be renewed
  name: ExpiresAt
  type: string
- description: Type or model of the registered device as reported during registration
  name: DeviceType
  type: string
- description: Subzone where the device is registered based on IP address ranges or alias patterns. Endpoints not matching any configured subzone are assigned to the DefaultSubzone.
  name: Subzone
  type: string
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-registration-schema.json
slug: cisco-expressway-registration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-search/cisco-expressway/json-schema/cisco-expressway-registration-schema.json\",\n  \"title\": \"Cisco Expressway Registration\",\n  \"description\": \"Schema for a device registration on Cisco Expressway. Represents an endpoint or device currently registered with the Expressway using SIP or H.323 protocols, including contact address, registration time, and subzone assignment.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alias\": {\n      \"type\": \"string\",\n      \"description\": \"Registered alias of the device, such as a SIP URI or H.323 alias\",\n      \"examples\": [\"user1@example.com\", \"alice.smith@company.com\"]\n    },\n    \"Type\": {\n      \"type\": \"string\",\n      \"description\": \"Registration protocol type\",\n      \"enum\": [\"SIP\", \"H.323\"]\n    },\n    \"ContactAddress\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Network contact address of the device, including IP address and port\",\n      \"examples\": [\"192.168.1.100:5060\", \"10.0.0.50:1720\"]\n    },\n    \"RegisteredAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the device registered\"\n    },\n    \"ExpiresAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"ISO 8601 timestamp when the registration expires and must be renewed\"\n    },\n    \"DeviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type or model of the registered device as reported during registration\",\n      \"examples\": [\"Cisco CE Software\", \"Cisco IP Phone 8845\", \"Jabber\"]\n    },\n    \"Subzone\": {\n      \"type\": \"string\",\n      \"description\": \"Subzone where the device is registered based on IP address ranges or alias patterns. Endpoints not matching any configured subzone are assigned to the DefaultSubzone.\",\n     \
  \ \"examples\": [\"DefaultSubzone\", \"HQ-Subzone\"]\n    }\n  },\n  \"required\": [\"Alias\", \"Type\", \"ContactAddress\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/json-schema/cisco-expressway-registration-schema.json
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway Registration
---
