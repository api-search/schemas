---
description: ''
layout: schema
name: MigrateZoneRequest
properties_list:
- description: Remote host to migrate the zone to
  name: host
  type: string
- description: Migration type
  name: type
  type: string
- description: Encryption cipher for the migration transfer
  name: cipher
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zones-management-migrate-zone-request-schema.json
slug: solaris-zones-management-migrate-zone-request
source_filename: solaris-zones-management-migrate-zone-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MigrateZoneRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Remote host to migrate the zone to\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Migration type\"\n    },\n    \"cipher\": {\n      \"type\": \"string\",\n      \"description\": \"Encryption cipher for the migration transfer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-migrate-zone-request-schema.json
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
title: MigrateZoneRequest
---
