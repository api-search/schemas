---
description: ''
layout: schema
name: LicenseInfo
properties_list:
- description: ''
  name: licenseType
  type: string
- description: Maximum number of concurrent call ports
  name: maxPorts
  type: integer
- description: Currently used call ports
  name: usedPorts
  type: integer
- description: Licensed feature list
  name: features
  type: array
- description: ''
  name: expirationDate
  type: string
- description: ''
  name: status
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-license-info-schema.json
slug: cisco-voice-portal-administration-license-info
source_filename: cisco-voice-portal-administration-license-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LicenseInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"licenseType\": {\n      \"type\": \"string\"\n    },\n    \"maxPorts\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number of concurrent call ports\"\n    },\n    \"usedPorts\": {\n      \"type\": \"integer\",\n      \"description\": \"Currently used call ports\"\n    },\n    \"features\": {\n      \"type\": \"array\",\n      \"description\": \"Licensed feature list\"\n    },\n    \"expirationDate\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-license-info-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: LicenseInfo
---
