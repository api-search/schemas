---
description: ''
layout: schema
name: StatisticIdentifier
properties_list:
- description: Statistics identifier in hierarchical namespace format (e.g., //:class:zones/zone-name/utilization/cpu)
  name: ssid
  type: string
- description: Statistic data type
  name: type
  type: string
- description: Human-readable description
  name: description
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-statistic-identifier-schema.json
slug: solaris-statsstore-statistic-identifier
source_filename: solaris-statsstore-statistic-identifier-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatisticIdentifier\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssid\": {\n      \"type\": \"string\",\n      \"description\": \"Statistics identifier in hierarchical namespace format (e.g., //:class:zones/zone-name/utilization/cpu)\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Statistic data type\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-statistic-identifier-schema.json
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
title: StatisticIdentifier
---
