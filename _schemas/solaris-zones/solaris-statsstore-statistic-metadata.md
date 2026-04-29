---
description: ''
layout: schema
name: StatisticMetadata
properties_list:
- description: Statistics identifier
  name: ssid
  type: string
- description: Human-readable description
  name: description
  type: string
- description: Data type
  name: type
  type: string
- description: Unit of measurement (e.g., bytes, percent, count)
  name: unit
  type: string
- description: Collection interval in seconds
  name: interval
  type: integer
- description: Whether historical data is retained
  name: persistent
  type: boolean
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-statistic-metadata-schema.json
slug: solaris-statsstore-statistic-metadata
source_filename: solaris-statsstore-statistic-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatisticMetadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssid\": {\n      \"type\": \"string\",\n      \"description\": \"Statistics identifier\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Data type\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement (e.g., bytes, percent, count)\"\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n      \"description\": \"Collection interval in seconds\"\n    },\n    \"persistent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether historical data is retained\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-statistic-metadata-schema.json
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
title: StatisticMetadata
---
