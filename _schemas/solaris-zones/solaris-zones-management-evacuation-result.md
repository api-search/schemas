---
description: ''
layout: schema
name: EvacuationResult
properties_list:
- description: Overall evacuation status
  name: status
  type: string
- description: Whether this is a return evacuation
  name: returning
  type: boolean
- description: Per-zone migration results keyed by zone name
  name: migrationResults
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zones-management-evacuation-result-schema.json
slug: solaris-zones-management-evacuation-result
source_filename: solaris-zones-management-evacuation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EvacuationResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall evacuation status\"\n    },\n    \"returning\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a return evacuation\"\n    },\n    \"migrationResults\": {\n      \"type\": \"object\",\n      \"description\": \"Per-zone migration results keyed by zone name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-evacuation-result-schema.json
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
title: EvacuationResult
---
