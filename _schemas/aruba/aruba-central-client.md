---
description: A client device connected to the network.
layout: schema
name: Client
properties_list:
- description: MAC address of the client.
  name: macaddr
  type: string
- description: Hostname or display name of the client.
  name: name
  type: string
- description: IP address assigned to the client.
  name: ip_address
  type: string
- description: Operating system type detected.
  name: os_type
  type: string
- description: Connection type.
  name: connection
  type: string
- description: SSID or network name the client is connected to.
  name: network
  type: string
- description: Radio band of the wireless connection.
  name: band
  type: number
- description: Channel number of the wireless connection.
  name: channel
  type: string
- description: Signal strength in dBm.
  name: signal_strength
  type: integer
- description: Signal-to-noise ratio in dB.
  name: signal_db
  type: integer
- description: Connection speed in Mbps.
  name: speed
  type: integer
- description: Serial number of the device the client is connected to.
  name: associated_device
  type: string
- description: Group name of the associated device.
  name: group_name
  type: string
- description: Site name of the associated device.
  name: site
  type: string
- description: Data usage statistics.
  name: usage
  type: object
provider_name: Aruba
provider_slug: aruba
schema_file: json-schema/aruba-central-client-schema.json
slug: aruba-central-client
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Client\",\n  \"type\": \"object\",\n  \"description\": \"A client device connected to the network.\",\n  \"properties\": {\n    \"macaddr\": {\n      \"type\": \"string\",\n      \"description\": \"MAC address of the client.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hostname or display name of the client.\"\n    },\n    \"ip_address\": {\n      \"type\": \"string\",\n      \"description\": \"IP address assigned to the client.\"\n    },\n    \"os_type\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system type detected.\"\n    },\n    \"connection\": {\n      \"type\": \"string\",\n      \"description\": \"Connection type.\"\n    },\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"SSID or network name the client is connected to.\"\n    },\n    \"band\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Radio band of the wireless connection.\"\n    },\n    \"channel\": {\n      \"type\": \"string\",\n      \"description\": \"Channel number of the wireless connection.\"\n    },\n    \"signal_strength\": {\n      \"type\": \"integer\",\n      \"description\": \"Signal strength in dBm.\"\n    },\n    \"signal_db\": {\n      \"type\": \"integer\",\n      \"description\": \"Signal-to-noise ratio in dB.\"\n    },\n    \"speed\": {\n      \"type\": \"integer\",\n      \"description\": \"Connection speed in Mbps.\"\n    },\n    \"associated_device\": {\n      \"type\": \"string\",\n      \"description\": \"Serial number of the device the client is connected to.\"\n    },\n    \"group_name\": {\n      \"type\": \"string\",\n      \"description\": \"Group name of the associated device.\"\n    },\n    \"site\": {\n      \"type\": \"string\",\n      \"description\": \"Site name of the associated device.\"\n    },\n    \"usage\": {\n      \"type\": \"object\",\n      \"description\": \"Data usage\
  \ statistics.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aruba/refs/heads/main/json-schema/aruba-central-client-schema.json
tags:
- Cloud
- Infrastructure
- Network Management
- Networking
- SD-WAN
- Security
- Switches
- Wireless
title: Client
---
