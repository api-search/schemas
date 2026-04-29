---
description: Device schema from Palo Alto Networks IoT Security API
layout: schema
name: Device
properties_list:
- description: Unique device identifier.
  name: deviceid
  type: string
- description: IPv4 address of the device.
  name: ip
  type: string
- description: MAC address of the device.
  name: mac
  type: string
- description: Hostname or NetBIOS name of the device.
  name: hostname
  type: string
- description: Device profile classification (e.g., IP Camera, Infusion Pump).
  name: profile
  type: string
- description: Device category (e.g., IoT, OT, IT).
  name: category
  type: string
- description: Aggregate risk score from 0 (lowest) to 100 (highest).
  name: risk_score
  type: integer
- description: Detected operating system.
  name: os
  type: string
- description: Detected operating system version.
  name: os_version
  type: string
- description: Device manufacturer or vendor.
  name: vendor
  type: string
- description: Device model identifier.
  name: model
  type: string
- description: Network site where the device was discovered.
  name: site
  type: string
- description: Subnet the device belongs to.
  name: subnet
  type: string
- description: Timestamp when the device was first discovered.
  name: first_seen
  type: string
- description: Timestamp when the device was last active.
  name: last_seen
  type: string
- description: Whether the device is currently monitored.
  name: monitored
  type: string
- description: Confidence level of the device profile classification.
  name: confidence_score
  type: integer
- description: User-defined or system-assigned tags.
  name: tags
  type: array
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/iot-security-api-device-schema.json
slug: iot-security-api-device
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Device\",\n  \"description\": \"Device schema from Palo Alto Networks IoT Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-device-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deviceid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique device identifier.\"\n    },\n    \"ip\": {\n      \"type\": \"string\",\n      \"format\": \"ipv4\",\n      \"description\": \"IPv4 address of the device.\"\n    },\n    \"mac\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the device.\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or NetBIOS name of the device.\"\n    },\n    \"profile\": {\n      \"type\": \"string\",\n      \"description\": \"Device profile classification (e.g., IP Camera, Infusion Pump).\"\
  \n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Device category (e.g., IoT, OT, IT).\"\n    },\n    \"risk_score\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"maximum\": 100,\n      \"description\": \"Aggregate risk score from 0 (lowest) to 100 (highest).\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"Detected operating system.\"\n    },\n    \"os_version\": {\n      \"type\": \"string\",\n      \"description\": \"Detected operating system version.\"\n    },\n    \"vendor\": {\n      \"type\": \"string\",\n      \"description\": \"Device manufacturer or vendor.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"Device model identifier.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Network site where the device was discovered.\"\n    },\n    \"subnet\": {\n      \"type\": \"string\",\n      \"description\": \"Subnet the device belongs\
  \ to.\"\n    },\n    \"first_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the device was first discovered.\"\n    },\n    \"last_seen\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the device was last active.\"\n    },\n    \"monitored\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"yes\",\n        \"no\"\n      ],\n      \"description\": \"Whether the device is currently monitored.\"\n    },\n    \"confidence_score\": {\n      \"type\": \"integer\",\n      \"description\": \"Confidence level of the device profile classification.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined or system-assigned tags.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-device-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: Device
---
