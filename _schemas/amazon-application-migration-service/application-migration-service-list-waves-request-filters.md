---
description: Filters for listing waves
layout: schema
name: ListWavesRequestFilters
properties_list:
- description: Filter by wave IDs
  name: waveIDs
  type: array
- description: Filter by archived status
  name: isArchived
  type: boolean
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-list-waves-request-filters-schema.json
slug: application-migration-service-list-waves-request-filters
source_filename: application-migration-service-list-waves-request-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-list-waves-request-filters-schema.json\",\n  \"title\": \"ListWavesRequestFilters\",\n  \"description\": \"Filters for listing waves\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waveIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by wave IDs\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Filter by archived status\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-list-waves-request-filters-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ListWavesRequestFilters
---
