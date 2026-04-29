---
description: Request to create a migration application
layout: schema
name: CreateApplicationRequest
properties_list:
- description: Application name
  name: name
  type: string
- description: Application description
  name: description
  type: string
- description: Tags for the application
  name: tags
  type: object
- description: Account ID for cross-account access
  name: accountID
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-create-application-request-schema.json
slug: application-migration-service-create-application-request
source_filename: application-migration-service-create-application-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-create-application-request-schema.json\",\n  \"title\": \"CreateApplicationRequest\",\n  \"description\": \"Request to create a migration application\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Application name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Application description\"\n    },\n    \"tags\": {\n      \"type\": \"object\",\n      \"description\": \"Tags for the application\"\n    },\n    \"accountID\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID for cross-account access\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-create-application-request-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: CreateApplicationRequest
---
