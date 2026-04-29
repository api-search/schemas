---
description: BatchDeleteImportDataRequest schema from Amazon Application Discovery Service API
layout: schema
name: BatchDeleteImportDataRequest
properties_list:
- description: The IDs for the import tasks that you want to delete.
  name: importTaskIds
  type: array
- description: Set to true to remove the deleted import task from Migration Hub.
  name: deleteHistory
  type: boolean
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-batch-delete-import-data-request-schema.json
slug: application-discovery-service-batch-delete-import-data-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-request-schema.json\",\n  \"title\": \"BatchDeleteImportDataRequest\",\n  \"description\": \"BatchDeleteImportDataRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"importTaskIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"maxItems\": 10,\n      \"example\": [\n        \"import-task-500123\"\n      ],\n      \"description\": \"The IDs for the import tasks that you want to delete.\"\n    },\n    \"deleteHistory\": {\n      \"type\": \"boolean\",\n      \"example\": false,\n      \"description\": \"Set to true to remove the deleted import task from Migration Hub.\"\n    }\n  },\n  \"required\": [\n    \"importTaskIds\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-batch-delete-import-data-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: BatchDeleteImportDataRequest
---
