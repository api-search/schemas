---
description: Request to delete a migration wave
layout: schema
name: DeleteWaveRequest
properties_list:
- description: Wave ID to delete
  name: waveID
  type: string
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-delete-wave-request-schema.json
slug: application-migration-service-delete-wave-request
source_filename: application-migration-service-delete-wave-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-delete-wave-request-schema.json\",\n  \"title\": \"DeleteWaveRequest\",\n  \"description\": \"Request to delete a migration wave\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"waveID\": {\n      \"type\": \"string\",\n      \"description\": \"Wave ID to delete\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-delete-wave-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: DeleteWaveRequest
---
