---
description: ''
layout: schema
name: MigrationError
properties_list:
- description: The operation that failed
  name: operation
  type: string
- description: System or zone configuration error
  name: error
  type: string
- description: Human-readable error message
  name: message
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zones-management-migration-error-schema.json
slug: solaris-zones-management-migration-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MigrationError\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operation\": {\n      \"type\": \"string\",\n      \"description\": \"The operation that failed\"\n    },\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"System or zone configuration error\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zones-management-migration-error-schema.json
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
title: MigrationError
---
