---
description: BatchDeleteImportDataError schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteImportDataError
properties_list:
- description: The unique import ID associated with the error that occurred.
  name: importTaskId
  type: string
- description: The type of error that occurred for a specific import task.
  name: errorCode
  type: string
- description: The description of the error that occurred for a specific import task.
  name: errorDescription
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-import-data-error-schema.json
slug: application-discovery-service-batch-delete-import-data-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-error-schema.json\",\n  \"title\": \"BatchDeleteImportDataError\",\n  \"description\": \"BatchDeleteImportDataError schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"importTaskId\": {\n      \"type\": \"string\",\n      \"example\": \"import-task-500123\",\n      \"description\": \"The unique import ID associated with the error that occurred.\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"example\": \"NOT_FOUND\",\n      \"description\": \"The type of error that occurred for a specific import task.\"\n    },\n    \"errorDescription\": {\n      \"type\": \"string\",\n      \"example\": \"Import task not found\",\n      \"description\": \"The description\
  \ of the error that occurred for a specific import task.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-error-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteImportDataError
---
