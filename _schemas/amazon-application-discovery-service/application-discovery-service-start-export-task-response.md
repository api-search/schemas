---
description: StartExportTaskResponse schema from Amazon Application Discovery Service API
layout: schema
name: StartExportTaskResponse
properties_list:
- description: A unique identifier used to query the status of an export request.
  name: exportId
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-export-task-response-schema.json
slug: application-discovery-service-start-export-task-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-export-task-response-schema.json\",\n  \"title\": \"StartExportTaskResponse\",\n  \"description\": \"StartExportTaskResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportId\": {\n      \"type\": \"string\",\n      \"example\": \"export-500123\",\n      \"description\": \"A unique identifier used to query the status of an export request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-export-task-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartExportTaskResponse
---
