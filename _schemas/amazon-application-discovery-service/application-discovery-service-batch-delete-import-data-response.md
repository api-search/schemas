---
description: BatchDeleteImportDataResponse schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteImportDataResponse
properties_list:
- description: Error messages returned for each import task that you deleted as a response for this command.
  name: errors
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-import-data-response-schema.json
slug: application-discovery-service-batch-delete-import-data-response
source_filename: application-discovery-service-batch-delete-import-data-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-response-schema.json\",\n  \"title\": \"BatchDeleteImportDataResponse\",\n  \"description\": \"BatchDeleteImportDataResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"importTaskId\": {\n            \"type\": \"string\",\n            \"example\": \"import-task-500123\",\n            \"description\": \"The unique import ID associated with the error that occurred.\"\n          },\n          \"errorCode\": {\n            \"type\": \"string\",\n            \"example\": \"NOT_FOUND\",\n            \"description\": \"The type of error that\
  \ occurred for a specific import task.\"\n          },\n          \"errorDescription\": {\n            \"type\": \"string\",\n            \"example\": \"Import task not found\",\n            \"description\": \"The description of the error that occurred for a specific import task.\"\n          }\n        }\n      },\n      \"description\": \"Error messages returned for each import task that you deleted as a response for this command.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteImportDataResponse
---
