---
description: StopContinuousExportRequest schema from Amazon Application Discovery Service API
layout: schema
name: StopContinuousExportRequest
properties_list:
- description: The unique ID assigned to this export.
  name: exportId
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-stop-continuous-export-request-schema.json
slug: application-discovery-service-stop-continuous-export-request
source_filename: application-discovery-service-stop-continuous-export-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-continuous-export-request-schema.json\",\n  \"title\": \"StopContinuousExportRequest\",\n  \"description\": \"StopContinuousExportRequest schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportId\": {\n      \"type\": \"string\",\n      \"example\": \"continuous-export-500123\",\n      \"description\": \"The unique ID assigned to this export.\"\n    }\n  },\n  \"required\": [\n    \"exportId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-continuous-export-request-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StopContinuousExportRequest
---
