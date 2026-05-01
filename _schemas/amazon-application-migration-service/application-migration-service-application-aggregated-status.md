---
description: Aggregated status of all source servers in an application
layout: schema
name: ApplicationAggregatedStatus
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
- description: Total number of source servers in the application
  name: totalSourceServers
  type: integer
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-application-aggregated-status-schema.json
slug: application-migration-service-application-aggregated-status
source_filename: application-migration-service-application-aggregated-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-application-aggregated-status-schema.json\",\n  \"title\": \"ApplicationAggregatedStatus\",\n  \"description\": \"Aggregated status of all source servers in an application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"lastUpdateDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of last status update\"\n    },\n    \"healthStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall health status\"\n    },\n    \"progressStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Overall progress status\"\n    },\n    \"totalSourceServers\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of source servers in the application\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-application-aggregated-status-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ApplicationAggregatedStatus
---
