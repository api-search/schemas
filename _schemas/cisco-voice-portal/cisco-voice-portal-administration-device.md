---
description: ''
layout: schema
name: Device
properties_list:
- description: Unique identifier for the device
  name: deviceId
  type: string
- description: Hostname of the device
  name: hostname
  type: string
- description: IP address of the device
  name: ipAddress
  type: string
- description: Type of CVP component
  name: deviceType
  type: string
- description: Device description
  name: description
  type: string
- description: Current operational status
  name: status
  type: string
- description: Software version installed on the device
  name: version
  type: string
- description: Last time the OAMP server contacted this device
  name: lastContact
  type: string
provider_name: Cisco Voice Portal
provider_slug: cisco-voice-portal
schema_file: json-schema/cisco-voice-portal-administration-device-schema.json
slug: cisco-voice-portal-administration-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Device\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the device\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname of the device\"\n    },\n    \"ipAddress\": {\n      \"type\": \"string\",\n      \"description\": \"IP address of the device\"\n    },\n    \"deviceType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of CVP component\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Device description\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Software version installed on the device\"\n    },\n    \"lastContact\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Last time the OAMP server contacted this device\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco-voice-portal/refs/heads/main/json-schema/cisco-voice-portal-administration-device-schema.json
tags:
- Contact Center
- IVR
- Telephony
- Voice
- VXML
title: Device
---
