---
description: PhysicalConnectionEntry schema from SP Interconnect Manage APIs
layout: schema
name: PhysicalConnectionEntry
properties_list:
- description: ''
  name: physicalConnectionName
  type: string
- description: ''
  name: linkType
  type: string
- description: ''
  name: requestedLinkCount
  type: integer
- description: ''
  name: coloFacilities
  type: array
- description: ''
  name: macSecEnabled
  type: boolean
- description: ''
  name: partnerName
  type: string
- description: ''
  name: partnerEmail
  type: string
provider_name: Palo Alto Networks
provider_slug: palo-alto-networks
schema_file: json-schema/sase-multitenant-interconnect-api-physical-connection-entry-schema.json
slug: sase-multitenant-interconnect-api-physical-connection-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PhysicalConnectionEntry\",\n  \"description\": \"PhysicalConnectionEntry schema from SP Interconnect Manage APIs\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-physical-connection-entry-schema.json\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"physicalConnectionName\": {\n      \"type\": \"string\",\n      \"pattern\": \"\\\\\\\\S\"\n    },\n    \"linkType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LINK_TYPE_ETHERNET_10G_LR\",\n        \"LINK_TYPE_ETHERNET_100G_LR\"\n      ]\n    },\n    \"requestedLinkCount\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"coloFacilities\": {\n      \"type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"macSecEnabled\": {\n      \"type\"\
  : \"boolean\"\n    },\n    \"partnerName\": {\n      \"type\": \"string\",\n      \"pattern\": \"\\\\\\\\S\"\n    },\n    \"partnerEmail\": {\n      \"type\": \"string\",\n      \"pattern\": \"\\\\\\\\S\"\n    }\n  },\n  \"required\": [\n    \"physicalConnectionName\",\n    \"linkType\",\n    \"coloFacilities\",\n    \"partnerName\",\n    \"partnerEmail\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/palo-alto-networks/refs/heads/main/json-schema/sase-multitenant-interconnect-api-physical-connection-entry-schema.json
tags:
- Cloud Security
- Cybersecurity
- Firewall
- Network Security
- SASE
- SOAR
- Threat Intelligence
- XDR
title: PhysicalConnectionEntry
---
