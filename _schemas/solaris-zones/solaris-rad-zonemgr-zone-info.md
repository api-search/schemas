---
description: Read-only snapshot of the executing zone information
layout: schema
name: ZoneInfo
properties_list:
- description: Name of the executing zone
  name: name
  type: string
- description: Numeric zone ID
  name: id
  type: integer
- description: Zone UUID
  name: uuid
  type: string
- description: Zone brand type
  name: brand
  type: string
- description: Whether this is the global zone
  name: isGlobal
  type: boolean
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-zone-info-schema.json
slug: solaris-rad-zonemgr-zone-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneInfo\",\n  \"type\": \"object\",\n  \"description\": \"Read-only snapshot of the executing zone information\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the executing zone\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Zone UUID\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand type\"\n    },\n    \"isGlobal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the global zone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-zone-info-schema.json
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
title: ZoneInfo
---
