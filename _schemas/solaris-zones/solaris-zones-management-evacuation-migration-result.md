---
description: ''
layout: schema
name: EvacuationMigrationResult
properties_list:
- description: Name of the zone
  name: zoneName
  type: string
- description: Whether the zone was successfully evacuated
  name: evacuated
  type: boolean
- description: Destination host
  name: evacuationTarget
  type: string
- description: Migration status
  name: migrationStatus
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zones-management-evacuation-migration-result-schema.json
slug: solaris-zones-management-evacuation-migration-result
source_filename: solaris-zones-management-evacuation-migration-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EvacuationMigrationResult\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone\"\n    },\n    \"evacuated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the zone was successfully evacuated\"\n    },\n    \"evacuationTarget\": {\n      \"type\": \"string\",\n      \"description\": \"Destination host\"\n    },\n    \"migrationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Migration status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-evacuation-migration-result-schema.json
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
title: EvacuationMigrationResult
---
