---
description: StartContinuousExportResponse schema from Amazon Application Discovery Service API
layout: schema
name: StartContinuousExportResponse
properties_list:
- description: The unique ID assigned to this export.
  name: exportId
  type: string
- description: The name of the s3 bucket where the export data parquet files are stored.
  name: s3Bucket
  type: string
- description: The timestamp representing when the continuous export was started.
  name: startTime
  type: string
- description: The type of data collector used to gather this data.
  name: dataSource
  type: string
- description: A dictionary which describes how the data is stored.
  name: schemaStorageConfig
  type: object
provider_name: Amazon Application Discovery Service
provider_slug: amazon-application-discovery-service
schema_file: json-schema/application-discovery-service-start-continuous-export-response-schema.json
slug: application-discovery-service-start-continuous-export-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-continuous-export-response-schema.json\",\n  \"title\": \"StartContinuousExportResponse\",\n  \"description\": \"StartContinuousExportResponse schema from Amazon Application Discovery Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"exportId\": {\n      \"type\": \"string\",\n      \"example\": \"continuous-export-500123\",\n      \"description\": \"The unique ID assigned to this export.\"\n    },\n    \"s3Bucket\": {\n      \"type\": \"string\",\n      \"example\": \"aws-application-discovery-service-500123\",\n      \"description\": \"The name of the s3 bucket where the export data parquet files are stored.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"example\": \"2026-04-19T10:00:00Z\",\n      \"description\"\
  : \"The timestamp representing when the continuous export was started.\"\n    },\n    \"dataSource\": {\n      \"type\": \"string\",\n      \"example\": \"AGENT\",\n      \"description\": \"The type of data collector used to gather this data.\"\n    },\n    \"schemaStorageConfig\": {\n      \"type\": \"object\",\n      \"description\": \"A dictionary which describes how the data is stored.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-application-discovery-service/refs/heads/main/json-schema/application-discovery-service-start-continuous-export-response-schema.json
tags:
- Amazon Application Discovery Service
- Migration
- Discovery
- Infrastructure
- AWS
title: StartContinuousExportResponse
---
