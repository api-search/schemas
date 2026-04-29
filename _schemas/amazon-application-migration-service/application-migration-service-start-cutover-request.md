---
description: Request to start a cutover migration job
layout: schema
name: StartCutoverRequest
properties_list:
- description: Source server IDs to cut over
  name: sourceServerIDs
  type: array
- description: Tags for the cutover job
  name: tags
  type: object
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-start-cutover-request-schema.json
slug: application-migration-service-start-cutover-request
source_filename: application-migration-service-start-cutover-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-start-cutover-request-schema.json\",\n  \"title\": \"StartCutoverRequest\",\n  \"description\": \"Request to start a cutover migration job\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"sourceServerIDs\": {\n      \"type\": \"array\",\n      \"description\": \"Source server IDs to cut over\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for the cutover job\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-start-cutover-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: StartCutoverRequest
---
