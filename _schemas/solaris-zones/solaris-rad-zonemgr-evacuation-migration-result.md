---
description: Migration result for an individual zone during evacuation
layout: schema
name: EvacuationMigrationResult
properties_list:
- description: Name of the evacuated zone
  name: zoneName
  type: string
- description: Whether the zone was successfully evacuated
  name: evacuated
  type: boolean
- description: Remote host where the zone was migrated
  name: evacuationTarget
  type: string
- description: Status of the individual zone migration
  name: migrationStatus
  type: string
- description: Error details if migration failed
  name: migrationError
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-rad-zonemgr-evacuation-migration-result-schema.json
slug: solaris-rad-zonemgr-evacuation-migration-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EvacuationMigrationResult\",\n  \"type\": \"object\",\n  \"description\": \"Migration result for an individual zone during evacuation\",\n  \"properties\": {\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the evacuated zone\"\n    },\n    \"evacuated\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the zone was successfully evacuated\"\n    },\n    \"evacuationTarget\": {\n      \"type\": \"string\",\n      \"description\": \"Remote host where the zone was migrated\"\n    },\n    \"migrationStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of the individual zone migration\"\n    },\n    \"migrationError\": {\n      \"type\": \"object\",\n      \"description\": \"Error details if migration failed\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-rad-zonemgr-evacuation-migration-result-schema.json
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
