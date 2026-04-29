---
description: ''
layout: schema
name: StatisticValue
properties_list:
- description: Statistics identifier
  name: ssid
  type: string
- description: Current value (type depends on the statistic)
  name: value
  type: string
- description: When the value was recorded
  name: timestamp
  type: string
- description: Unit of measurement
  name: unit
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-statistic-value-schema.json
slug: solaris-statsstore-statistic-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatisticValue\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssid\": {\n      \"type\": \"string\",\n      \"description\": \"Statistics identifier\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Current value (type depends on the statistic)\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"description\": \"When the value was recorded\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-statistic-value-schema.json
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
title: StatisticValue
---
