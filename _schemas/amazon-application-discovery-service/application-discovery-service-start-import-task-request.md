---
description: StartImportTaskRequest schema from Amazon Application Discovery Service API
layout: schema
name: StartImportTaskRequest
properties_list:
- description: Optional. A unique token that you can provide to prevent the same import request from occurring more than once.
  name: clientRequestToken
  type: string
- description: A descriptive name for this request. You can use this name to filter future requests related to this import task, such as identifying applications and servers that were included in this import task.
  name: name
  type: string
- description: The URL for your import file that you've uploaded to Amazon S3.
  name: importUrl
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-import-task-request-schema.json
slug: application-discovery-service-start-import-task-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-import-task-request-schema.json\",\n  \"title\": \"StartImportTaskRequest\",\n  \"description\": \"StartImportTaskRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clientRequestToken\": {\n      \"type\": \"string\",\n      \"example\": \"client-token-500123\",\n      \"description\": \"Optional. A unique token that you can provide to prevent the same import request from occurring more than once.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"maxLength\": 255,\n      \"example\": \"Server Inventory Import April 2026\",\n      \"description\": \"A descriptive name for this request. You can use this name to filter future requests related to this import task, such as\
  \ identifying applications and servers that were included in this import task.\"\n    },\n    \"importUrl\": {\n      \"type\": \"string\",\n      \"example\": \"s3://my-bucket/server-inventory.csv\",\n      \"description\": \"The URL for your import file that you've uploaded to Amazon S3.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"importUrl\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-import-task-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartImportTaskRequest
---
