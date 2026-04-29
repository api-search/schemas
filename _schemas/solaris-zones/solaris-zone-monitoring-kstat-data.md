---
description: ''
layout: schema
name: KstatData
properties_list:
- description: ''
  name: module
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: statistic
  type: string
- description: ''
  name: instance
  type: integer
- description: Snapshot time in nanoseconds
  name: snaptime
  type: integer
- description: Key-value pairs of statistic data
  name: data
  type: object
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-monitoring-kstat-data-schema.json
slug: solaris-zone-monitoring-kstat-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"KstatData\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"module\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"statistic\": {\n      \"type\": \"string\"\n    },\n    \"instance\": {\n      \"type\": \"integer\"\n    },\n    \"snaptime\": {\n      \"type\": \"integer\",\n      \"description\": \"Snapshot time in nanoseconds\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value pairs of statistic data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-kstat-data-schema.json
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
title: KstatData
---
