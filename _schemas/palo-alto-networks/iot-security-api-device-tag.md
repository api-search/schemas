---
description: DeviceTag schema from Palo Alto Networks IoT Security API
layout: schema
name: DeviceTag
properties_list:
- description: Unique tag identifier.
  name: id
  type: string
- description: Tag name.
  name: name
  type: string
- description: Tag description.
  name: description
  type: string
- description: Number of devices assigned this tag.
  name: device_count
  type: integer
- description: Timestamp when the tag was created.
  name: created_at
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/iot-security-api-device-tag-schema.json
slug: iot-security-api-device-tag
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeviceTag\",\n  \"description\": \"DeviceTag schema from Palo Alto Networks IoT Security API\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-device-tag-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique tag identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Tag name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Tag description.\"\n    },\n    \"device_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of devices assigned this tag.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the tag was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/iot-security-api-device-tag-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: DeviceTag
---
