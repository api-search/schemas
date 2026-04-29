---
description: A Meraki network.
layout: schema
name: Network
properties_list:
- description: Network ID.
  name: id
  type: string
- description: Organization ID.
  name: organizationId
  type: string
- description: Network name.
  name: name
  type: string
- description: Product types in the network.
  name: productTypes
  type: array
- description: Timezone of the network.
  name: timeZone
  type: string
- description: Tags applied to the network.
  name: tags
  type: array
provider_name: Cisco
provider_slug: cisco
schema_file: json-schema/cisco-meraki-api-network-schema.json
slug: cisco-meraki-api-network
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-network-schema.json\",\n  \"title\": \"Network\",\n  \"description\": \"A Meraki network.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"string\", \"description\": \"Network ID.\" },\n    \"organizationId\": { \"type\": \"string\", \"description\": \"Organization ID.\" },\n    \"name\": { \"type\": \"string\", \"description\": \"Network name.\" },\n    \"productTypes\": { \"type\": \"array\", \"items\": { \"type\": \"string\" }, \"description\": \"Product types in the network.\" },\n    \"timeZone\": { \"type\": \"string\", \"description\": \"Timezone of the network.\" },\n    \"tags\": { \"type\": \"array\", \"items\": { \"type\": \"string\" }, \"description\": \"Tags applied to the network.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cisco/refs/heads/main/json-schema/cisco-meraki-api-network-schema.json
tags:
- Collaboration
- Enterprise
- Networking
- Security
- SD-WAN
title: Network
---
