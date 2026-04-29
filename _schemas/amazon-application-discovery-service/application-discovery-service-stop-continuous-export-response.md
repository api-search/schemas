---
description: StopContinuousExportResponse schema from Amazon Application Discovery Service API
layout: schema
name: StopContinuousExportResponse
properties_list:
- description: Timestamp that represents when this continuous export started collecting data.
  name: startTime
  type: string
- description: Timestamp that represents when this continuous export was stopped.
  name: stopTime
  type: string
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-stop-continuous-export-response-schema.json
slug: application-discovery-service-stop-continuous-export-response
source_filename: application-discovery-service-stop-continuous-export-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-continuous-export-response-schema.json\",\n  \"title\": \"StopContinuousExportResponse\",\n  \"description\": \"StopContinuousExportResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:00:00Z\",\n      \"description\": \"Timestamp that represents when this continuous export started collecting data.\"\n    },\n    \"stopTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T11:00:00Z\",\n      \"description\": \"Timestamp that represents when this continuous export was stopped.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-stop-continuous-export-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StopContinuousExportResponse
---
