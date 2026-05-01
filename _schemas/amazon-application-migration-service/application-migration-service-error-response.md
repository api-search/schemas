---
description: Standard error response from the Application Migration Service API
layout: schema
name: ErrorResponse
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-error-response-schema.json
slug: application-migration-service-error-response
source_filename: application-migration-service-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-error-response-schema.json\",\n  \"title\": \"ErrorResponse\",\n  \"description\": \"Standard error response from the Application Migration Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-error-response-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- Cloud Migration
title: ErrorResponse
---
