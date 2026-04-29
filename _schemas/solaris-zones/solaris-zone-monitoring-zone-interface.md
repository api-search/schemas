---
description: ''
layout: schema
name: ZoneInterface
properties_list:
- description: URL path to the zone interface
  name: href
  type: string
- description: Interface type (Zone, ZoneInfo, ZoneManager)
  name: type
  type: string
- description: Zone name
  name: name
  type: string
- description: Current zone state
  name: state
  type: string
- description: Zone brand
  name: brand
  type: string
- description: Zone numeric ID
  name: id
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-monitoring-zone-interface-schema.json
slug: solaris-zone-monitoring-zone-interface
source_filename: solaris-zone-monitoring-zone-interface-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneInterface\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"URL path to the zone interface\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Interface type (Zone, ZoneInfo, ZoneManager)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current zone state\"\n    },\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Zone numeric ID\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-zone-interface-schema.json
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
title: ZoneInterface
---
