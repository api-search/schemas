---
description: Device information returned by the GetDevInfo command including model, firmware, hardware version, and capabilities.
layout: schema
name: Reolink Device Info
properties_list:
- description: RS485 support flag
  name: B485
  type: integer
- description: Number of IO input ports
  name: IOInputNum
  type: integer
- description: Number of IO output ports
  name: IOOutputNum
  type: integer
- description: Number of audio channels
  name: audioNum
  type: integer
- description: Firmware build date
  name: buildDay
  type: string
- description: Configuration version
  name: cfgVer
  type: string
- description: Number of camera channels
  name: channelNum
  type: integer
- description: Device detail string
  name: detail
  type: string
- description: Number of disk slots
  name: diskNum
  type: integer
- description: Firmware version string
  name: firmVer
  type: string
- description: Framework version number
  name: frameworkVer
  type: integer
- description: Hardware version string
  name: hardVer
  type: string
- description: Device model name
  name: model
  type: string
- description: Device display name
  name: name
  type: string
- description: Firmware package suffix
  name: pakSuffix
  type: string
- description: Device serial number
  name: serial
  type: string
- description: Device type identifier
  name: type
  type: string
- description: WiFi support flag (0 or 1)
  name: wifi
  type: integer
provider_name: Reolink
provider_slug: reolink
schema_file: json-schema/device-info.json
slug: device-info
source_filename: device-info.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"device-info.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Reolink Device Info\",\n  \"description\": \"Device information returned by the GetDevInfo command including model, firmware, hardware version, and capabilities.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"B485\": {\n      \"type\": \"integer\",\n      \"description\": \"RS485 support flag\"\n    },\n    \"IOInputNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of IO input ports\"\n    },\n    \"IOOutputNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of IO output ports\"\n    },\n    \"audioNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of audio channels\"\n    },\n    \"buildDay\": {\n      \"type\": \"string\",\n      \"description\": \"Firmware build date\"\n    },\n    \"cfgVer\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration version\"\n    },\n \
  \   \"channelNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of camera channels\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"description\": \"Device detail string\"\n    },\n    \"diskNum\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of disk slots\"\n    },\n    \"firmVer\": {\n      \"type\": \"string\",\n      \"description\": \"Firmware version string\"\n    },\n    \"frameworkVer\": {\n      \"type\": \"integer\",\n      \"description\": \"Framework version number\"\n    },\n    \"hardVer\": {\n      \"type\": \"string\",\n      \"description\": \"Hardware version string\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Device model name\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Device display name\"\n    },\n    \"pakSuffix\": {\n      \"type\": \"string\",\n      \"description\": \"Firmware package suffix\"\n    },\n    \"serial\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"Device serial number\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Device type identifier\"\n    },\n    \"wifi\": {\n      \"type\": \"integer\",\n      \"description\": \"WiFi support flag (0 or 1)\"\n    }\n  },\n  \"required\": [\"model\", \"firmVer\", \"hardVer\", \"name\", \"serial\", \"type\", \"channelNum\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reolink/refs/heads/main/json-schema/device-info.json
tags:
- IoT
- Security Cameras
- Surveillance
- Smart Home
- AI Detection
title: Reolink Device Info
---
