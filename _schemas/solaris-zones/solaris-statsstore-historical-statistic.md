---
description: ''
layout: schema
name: HistoricalStatistic
properties_list:
- description: Statistics identifier
  name: ssid
  type: string
- description: Time series data points
  name: dataPoints
  type: array
- description: Unit of measurement
  name: unit
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-statsstore-historical-statistic-schema.json
slug: solaris-statsstore-historical-statistic
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HistoricalStatistic\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ssid\": {\n      \"type\": \"string\",\n      \"description\": \"Statistics identifier\"\n    },\n    \"dataPoints\": {\n      \"type\": \"array\",\n      \"description\": \"Time series data points\"\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measurement\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-statsstore-historical-statistic-schema.json
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
title: HistoricalStatistic
---
