---
description: Represents a multi-zone evacuation operation in Oracle Solaris, including overall status, per-zone migration results, and progress tracking for evacuating zones from one host to another. Available since RAD zonemgr API version 1.4.
layout: schema
name: Oracle Solaris Zone Evacuation
properties_list:
- description: Overall evacuation status
  name: status
  type: string
- description: Whether this is a return evacuation (zones being moved back to original host)
  name: returning
  type: boolean
- description: Per-zone migration results keyed by zone name
  name: migrationResults
  type: object
- description: ''
  name: progress
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-evacuation-schema.json
slug: solaris-zone-evacuation
source_filename: solaris-zone-evacuation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-evacuation.json\",\n  \"title\": \"Oracle Solaris Zone Evacuation\",\n  \"description\": \"Represents a multi-zone evacuation operation in Oracle Solaris, including overall status, per-zone migration results, and progress tracking for evacuating zones from one host to another. Available since RAD zonemgr API version 1.4.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall evacuation status\",\n      \"enum\": [\"SUCCESS\", \"FAIL\", \"PARTIAL_FAIL\"]\n    },\n    \"returning\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a return evacuation (zones being moved back to original host)\"\n    },\n    \"migrationResults\": {\n      \"type\": \"object\",\n      \"description\": \"Per-zone migration results keyed by zone name\",\n      \"additionalProperties\"\
  : {\n        \"$ref\": \"#/$defs/EvacuationMigrationResult\"\n      }\n    },\n    \"progress\": {\n      \"$ref\": \"#/$defs/EvacuationProgress\"\n    }\n  },\n  \"$defs\": {\n    \"EvacuationMigrationResult\": {\n      \"type\": \"object\",\n      \"description\": \"Migration result for a single zone during evacuation\",\n      \"properties\": {\n        \"zoneName\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the evacuated zone\"\n        },\n        \"evacuated\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether the zone was successfully evacuated\"\n        },\n        \"evacuationTarget\": {\n          \"type\": \"string\",\n          \"description\": \"Destination host the zone was evacuated to\"\n        },\n        \"migrationStatus\": {\n          \"type\": \"string\",\n          \"description\": \"Migration status for this zone\"\n        },\n        \"migrationError\": {\n          \"type\": [\"object\", \"null\"],\n  \
  \        \"description\": \"Error details if migration failed\",\n          \"properties\": {\n            \"operation\": {\n              \"type\": \"string\",\n              \"description\": \"The operation that failed\"\n            },\n            \"error\": {\n              \"type\": [\"string\", \"null\"],\n              \"description\": \"Error code\"\n            },\n            \"message\": {\n              \"type\": \"string\",\n              \"description\": \"Error message\"\n            }\n          }\n        }\n      }\n    },\n    \"EvacuationProgress\": {\n      \"type\": \"object\",\n      \"description\": \"Progress information for an ongoing evacuation\",\n      \"properties\": {\n        \"zoneName\": {\n          \"type\": \"string\",\n          \"description\": \"Zone currently being evacuated\"\n        },\n        \"remoteHost\": {\n          \"type\": \"string\",\n          \"description\": \"Destination host\"\n        },\n        \"returning\": {\n         \
  \ \"type\": \"boolean\",\n          \"description\": \"Whether this is a return evacuation\"\n        },\n        \"migrationMilestone\": {\n          \"type\": \"string\",\n          \"description\": \"Current migration milestone\",\n          \"enum\": [\n            \"MIGRATE_INITIALIZING\",\n            \"MIGRATE_INITIALIZATION_COMPLETE\",\n            \"MIGRATE_INITIALIZATION_FAIL\",\n            \"MIGRATING\",\n            \"MIGRATE_COMPLETE\",\n            \"MIGRATE_FAIL\",\n            \"EVACUATE_INITIALIZING\",\n            \"EVACUATE_INITIALIZATION_COMPLETE\",\n            \"EVACUATE_INITIALIZATION_FAIL\",\n            \"EVACUATING\",\n            \"EVACUATE_COMPLETE\",\n            \"EVACUATE_FAIL\",\n            \"EVACUATE_CANCELED\"\n          ]\n        },\n        \"zoneCount\": {\n          \"type\": \"integer\",\n          \"description\": \"Total number of zones being evacuated\",\n          \"minimum\": 0\n        },\n        \"transferRate\": {\n          \"type\":\
  \ [\"integer\", \"null\"],\n          \"description\": \"Current transfer rate in bytes per second\"\n        },\n        \"zoneProgress\": {\n          \"type\": \"string\",\n          \"description\": \"Detailed progress information for the current zone\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-evacuation-schema.json
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
title: Oracle Solaris Zone Evacuation
---
