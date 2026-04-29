---
description: Detailed information about a specific Solaris zone
layout: schema
name: ZoneDetail
properties_list:
- description: Zone name
  name: name
  type: string
- description: Zone numeric ID assigned by the kernel when the zone is running
  name: id
  type: integer
- description: Universally unique identifier for the zone
  name: uuid
  type: string
- description: Current zone state
  name: state
  type: string
- description: Zone brand determining the runtime environment
  name: brand
  type: string
- description: Auxiliary state information for the zone
  name: auxstate
  type: array
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-zone-detail-schema.json
slug: solaris-rad-zonemgr-zone-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneDetail\",\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a specific Solaris zone\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Zone numeric ID assigned by the kernel when the zone is running\"\n    },\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Universally unique identifier for the zone\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current zone state\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand determining the runtime environment\"\n    },\n    \"auxstate\": {\n      \"type\": \"array\",\n      \"description\": \"Auxiliary state information for the zone\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-zone-detail-schema.json
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
title: ZoneDetail
---
