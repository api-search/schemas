---
description: Device identifier for connectivity status queries
layout: schema
name: Device
properties_list:
- description: Mobile phone number in E.164 format
  name: phoneNumber
  type: string
- description: Device IPv4 address (alternative to phoneNumber)
  name: ipv4Address
  type: object
- description: Network access identifier (alternative to phoneNumber)
  name: networkAccessIdentifier
  type: string
provider_name: AT&T Developer Hub
provider_slug: at-t-developer-hub
schema_file: json-schema/device-status-api-device-schema.json
slug: device-status-api-device
tags:
- 5G
- Network APIs
- CAMARA
- Connectivity
- Telecommunications
- Edge Computing
- Device Status
- SIM Swap
title: Device
---
