---
description: Aggregated status of all applications in a wave
layout: schema
name: WaveAggregatedStatus
properties_list:
- description: Date/time of last status update
  name: lastUpdateDateTime
  type: string
- description: Overall health status
  name: healthStatus
  type: string
- description: Overall progress status
  name: progressStatus
  type: string
- description: Total number of applications in the wave
  name: totalApplications
  type: integer
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-wave-aggregated-status-schema.json
slug: application-migration-service-wave-aggregated-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-wave-aggregated-status-schema.json\",\n  \"title\": \"WaveAggregatedStatus\",\n  \"description\": \"Aggregated status of all applications in a wave\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastUpdateDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of last status update\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall health status\"\n    },\n    \"progressStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall progress status\"\n    },\n    \"totalApplications\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of applications in the wave\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-wave-aggregated-status-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: WaveAggregatedStatus
---
