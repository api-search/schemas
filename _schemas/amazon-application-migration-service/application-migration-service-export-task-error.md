---
description: An error from a source server export task
layout: schema
name: ExportTaskError
properties_list:
- description: errorData
  name: errorData
  type: string
- description: Date/time of the error
  name: errorDateTime
  type: string
provider_name: Amazon Application Migration Service
provider_slug: amazon-application-migration-service
schema_file: json-schema/application-migration-service-export-task-error-schema.json
slug: application-migration-service-export-task-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-application-migration-service/json-schema/application-migration-service-export-task-error-schema.json\",\n  \"title\": \"ExportTaskError\",\n  \"description\": \"An error from a source server export task\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errorData\": {\n      \"type\": \"string\",\n      \"description\": \"errorData\"\n    },\n    \"errorDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"Date/time of the error\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-migration-service/refs/heads/main/json-schema/application-migration-service-export-task-error-schema.json
tags:
- Amazon Application Migration Service
- Migration
- Lift And Shift
- AWS
- Cloud Migration
title: ExportTaskError
---
