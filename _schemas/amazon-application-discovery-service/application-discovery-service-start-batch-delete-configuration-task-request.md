---
description: StartBatchDeleteConfigurationTaskRequest schema from Amazon Application Discovery Service API
layout: schema
name: StartBatchDeleteConfigurationTaskRequest
properties_list:
- description: The type of configuration item to delete. Supported types are SERVER.
  name: configurationType
  type: string
- description: The list of configuration IDs that will be deleted by this task.
  name: configurationIds
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-batch-delete-configuration-task-request-schema.json
slug: application-discovery-service-start-batch-delete-configuration-task-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-batch-delete-configuration-task-request-schema.json\",\n  \"title\": \"StartBatchDeleteConfigurationTaskRequest\",\n  \"description\": \"StartBatchDeleteConfigurationTaskRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"configurationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SERVER\"\n      ],\n      \"example\": \"SERVER\",\n      \"description\": \"The type of configuration item to delete. Supported types are SERVER.\"\n    },\n    \"configurationIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"d-SERVER-500456\"\n      ],\n      \"description\": \"The list of configuration\
  \ IDs that will be deleted by this task.\"\n    }\n  },\n  \"required\": [\n    \"configurationType\",\n    \"configurationIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-batch-delete-configuration-task-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartBatchDeleteConfigurationTaskRequest
---
