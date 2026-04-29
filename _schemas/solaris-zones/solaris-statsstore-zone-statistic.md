---
description: ''
layout: schema
name: ZoneStatistic
properties_list:
- description: Zone name
  name: zoneName
  type: string
- description: Numeric zone ID
  name: zoneId
  type: integer
- description: Metric name
  name: metric
  type: string
- description: Current metric value
  name: value
  type: number
- description: Unit of measurement
  name: unit
  type: string
- description: When the value was recorded
  name: timestamp
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-zone-statistic-schema.json
slug: solaris-statsstore-zone-statistic
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneStatistic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zoneName\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"zoneId\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID\"\n    },\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"Metric name\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Current metric value\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"When the value was recorded\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-zone-statistic-schema.json
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
title: ZoneStatistic
---
