---
description: ''
layout: schema
name: KernelZone
properties_list:
- description: Kernel zone name
  name: name
  type: string
- description: Zone brand (solaris-kz for kernel zones)
  name: brand
  type: string
- description: Numeric zone ID
  name: id
  type: integer
- description: Zone UUID
  name: uuid
  type: string
- description: Current zone state
  name: state
  type: string
- description: Auxiliary zone states
  name: auxstate
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-kernel-zones-kernel-zone-schema.json
slug: solaris-kernel-zones-kernel-zone
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KernelZone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Kernel zone name\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand (solaris-kz for kernel zones)\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Zone UUID\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current zone state\"\n    },\n    \"auxstate\": {\n      \"type\": \"array\",\n      \"description\": \"Auxiliary zone states\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-kernel-zones-kernel-zone-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: KernelZone
---
