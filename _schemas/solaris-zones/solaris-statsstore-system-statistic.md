---
description: ''
layout: schema
name: SystemStatistic
properties_list:
- description: System metric name
  name: metric
  type: string
- description: Current metric value
  name: value
  type: number
- description: Unit of measurement
  name: unit
  type: string
- description: ''
  name: timestamp
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-system-statistic-schema.json
slug: solaris-statsstore-system-statistic
source_filename: solaris-statsstore-system-statistic-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SystemStatistic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metric\": {\n      \"type\": \"string\",\n      \"description\": \"System metric name\"\n    },\n    \"value\": {\n      \"type\": \"number\",\n      \"description\": \"Current metric value\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-system-statistic-schema.json
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
title: SystemStatistic
---
