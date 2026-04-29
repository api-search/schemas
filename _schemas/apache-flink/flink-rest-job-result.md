---
description: JobResult schema from Apache Flink REST API
layout: schema
name: JobResult
properties_list:
- description: ''
  name: accumulatorResults
  type: object
- description: ''
  name: applicationStatus
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: netRuntime
  type: integer
- description: ''
  name: serializedThrowable
  type: object
- description: ''
  name: success
  type: boolean
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-result-schema.json
slug: flink-rest-job-result
source_filename: flink-rest-job-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-result-schema.json\",\n  \"title\": \"JobResult\",\n  \"description\": \"JobResult schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accumulatorResults\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"$ref\": \"#/components/schemas/SerializedValueOptionalFailureObject\"\n      }\n    },\n    \"applicationStatus\": {\n      \"$ref\": \"#/components/schemas/ApplicationStatus\"\n    },\n    \"jobId\": {\n      \"$ref\": \"#/components/schemas/JobID\"\n    },\n    \"netRuntime\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"serializedThrowable\": {\n      \"$ref\": \"#/components/schemas/SerializedThrowable\"\n    },\n    \"success\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-result-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobResult
---
