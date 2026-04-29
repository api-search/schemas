---
description: A Meraki network device.
layout: schema
name: Device
properties_list:
- description: Device serial number.
  name: serial
  type: string
- description: Device name.
  name: name
  type: string
- description: Device MAC address.
  name: mac
  type: string
- description: Device model.
  name: model
  type: string
- description: Network ID.
  name: networkId
  type: string
- description: LAN IP address.
  name: lanIp
  type: string
- description: Firmware version.
  name: firmware
  type: string
provider_name: Cisco
provider_slug: cisco
schema_file: json-schema/cisco-meraki-api-device-schema.json
slug: cisco-meraki-api-device
source_filename: cisco-meraki-api-device-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-device-schema.json\",\n  \"title\": \"Device\",\n  \"description\": \"A Meraki network device.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serial\": { \"type\": \"string\", \"description\": \"Device serial number.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Device name.\" },\n    \"mac\": { \"type\": \"string\", \"description\": \"Device MAC address.\" },\n    \"model\": { \"type\": \"string\", \"description\": \"Device model.\" },\n    \"networkId\": { \"type\": \"string\", \"description\": \"Network ID.\" },\n    \"lanIp\": { \"type\": \"string\", \"description\": \"LAN IP address.\" },\n    \"firmware\": { \"type\": \"string\", \"description\": \"Firmware version.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-device-schema.json
tags:
- Collaboration
- Enterprise
- Networking
- Security
- SD-WAN
title: Device
---
