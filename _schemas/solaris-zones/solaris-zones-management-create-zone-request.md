---
description: ''
layout: schema
name: CreateZoneRequest
properties_list:
- description: Name of the new zone
  name: name
  type: string
- description: Zone root path
  name: path
  type: string
- description: Zone brand template (e.g., SYSdefault)
  name: template
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zones-management-create-zone-request-schema.json
slug: solaris-zones-management-create-zone-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateZoneRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the new zone\"\n    },\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Zone root path\"\n    },\n    \"template\": {\n      \"type\": \"string\",\n      \"description\": \"Zone brand template (e.g., SYSdefault)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-create-zone-request-schema.json
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
title: CreateZoneRequest
---
