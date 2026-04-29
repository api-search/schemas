---
description: Filters for listing applications
layout: schema
name: ListApplicationsRequestFilters
properties_list:
- description: Filter by application IDs
  name: applicationIDs
  type: array
- description: Filter by archived status
  name: isArchived
  type: boolean
- description: Filter by wave IDs
  name: waveIDs
  type: array
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-list-applications-request-filters-schema.json
slug: application-migration-service-list-applications-request-filters
source_filename: application-migration-service-list-applications-request-filters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-list-applications-request-filters-schema.json\",\n  \"title\": \"ListApplicationsRequestFilters\",\n  \"description\": \"Filters for listing applications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by application IDs\"\n    },\n    \"isArchived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Filter by archived status\"\n    },\n    \"waveIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Filter by wave IDs\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-list-applications-request-filters-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: ListApplicationsRequestFilters
---
