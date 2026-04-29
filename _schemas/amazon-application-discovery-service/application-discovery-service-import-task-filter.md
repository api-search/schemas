---
description: ImportTaskFilter schema from Amazon Application Discovery Service API
layout: schema
name: ImportTaskFilter
properties_list:
- description: The name, status, or import task ID for a specific import task.
  name: name
  type: string
- description: An array of strings that you can provide to match against a specific name, status, or import task ID to filter your import task.
  name: values
  type: array
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-import-task-filter-schema.json
slug: application-discovery-service-import-task-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-import-task-filter-schema.json\",\n  \"title\": \"ImportTaskFilter\",\n  \"description\": \"ImportTaskFilter schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"IMPORT_TASK_ID\",\n        \"STATUS\",\n        \"NAME\"\n      ],\n      \"example\": \"STATUS\",\n      \"description\": \"The name, status, or import task ID for a specific import task.\"\n    },\n    \"values\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"IMPORT_COMPLETE\"\n      ],\n      \"description\": \"An array of strings that you can provide to match against a specific name, status,\
  \ or import task ID to filter your import task.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-import-task-filter-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: ImportTaskFilter
---
