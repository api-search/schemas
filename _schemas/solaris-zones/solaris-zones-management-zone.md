---
description: ''
layout: schema
name: Zone
properties_list:
- description: Zone name
  name: name
  type: string
- description: Zone brand type (e.g., solaris, solaris-kz, solaris10)
  name: brand
  type: string
- description: Numeric zone ID (only when running or ready)
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
schema_file: json-schema/solaris-zones-management-zone-schema.json
slug: solaris-zones-management-zone
source_filename: solaris-zones-management-zone-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Zone\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand type (e.g., solaris, solaris-kz, solaris10)\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID (only when running or ready)\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Zone UUID\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current zone state\"\n    },\n    \"auxstate\": {\n      \"type\": \"array\",\n      \"description\": \"Auxiliary zone states\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-zone-schema.json
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
title: Zone
---
