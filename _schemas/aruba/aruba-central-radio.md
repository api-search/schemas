---
description: Radio interface on an access point.
layout: schema
name: Radio
properties_list:
- description: Radio index (0 or 1).
  name: index
  type: integer
- description: MAC address of the radio interface.
  name: macaddr
  type: string
- description: Operating frequency band in GHz.
  name: band
  type: number
- description: Operating channel number.
  name: channel
  type: string
- description: Transmit power in dBm.
  name: power
  type: integer
- description: Effective transmit power in dBm.
  name: tx_power
  type: integer
- description: Channel utilization percentage.
  name: utilization
  type: integer
- description: Noise floor in dBm.
  name: noise_floor
  type: integer
- description: Radio operational status.
  name: status
  type: string
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-radio-schema.json
slug: aruba-central-radio
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Radio\",\n  \"type\": \"object\",\n  \"description\": \"Radio interface on an access point.\",\n  \"properties\": {\n    \"index\": {\n      \"type\": \"integer\",\n      \"description\": \"Radio index (0 or 1).\"\n    },\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the radio interface.\"\n    },\n    \"band\": {\n      \"type\": \"number\",\n      \"description\": \"Operating frequency band in GHz.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"Operating channel number.\"\n    },\n    \"power\": {\n      \"type\": \"integer\",\n      \"description\": \"Transmit power in dBm.\"\n    },\n    \"tx_power\": {\n      \"type\": \"integer\",\n      \"description\": \"Effective transmit power in dBm.\"\n    },\n    \"utilization\": {\n      \"type\": \"integer\",\n      \"description\": \"Channel utilization percentage.\"\
  \n    },\n    \"noise_floor\": {\n      \"type\": \"integer\",\n      \"description\": \"Noise floor in dBm.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Radio operational status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-radio-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Radio
---
