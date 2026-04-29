---
description: JarRunRequestBody schema from Apache Flink REST API
layout: schema
name: JarRunRequestBody
properties_list:
- description: ''
  name: allowNonRestoredState
  type: boolean
- description: ''
  name: claimMode
  type: object
- description: ''
  name: entryClass
  type: string
- description: ''
  name: flinkConfiguration
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: parallelism
  type: integer
- description: ''
  name: programArgsList
  type: array
- description: ''
  name: restoreMode
  type: object
- description: ''
  name: savepointPath
  type: string
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-jar-run-request-body-schema.json
slug: flink-rest-jar-run-request-body
source_filename: flink-rest-jar-run-request-body-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jar-run-request-body-schema.json\",\n  \"title\": \"JarRunRequestBody\",\n  \"description\": \"JarRunRequestBody schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowNonRestoredState\": {\n      \"type\": \"boolean\"\n    },\n    \"claimMode\": {\n      \"$ref\": \"#/components/schemas/RecoveryClaimMode\"\n    },\n    \"entryClass\": {\n      \"type\": \"string\"\n    },\n    \"flinkConfiguration\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"jobId\": {\n      \"$ref\": \"#/components/schemas/JobID\"\n    },\n    \"parallelism\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"programArgsList\": {\n      \"type\": \"array\",\n      \"items\": {\n    \
  \    \"type\": \"string\"\n      }\n    },\n    \"restoreMode\": {\n      \"$ref\": \"#/components/schemas/RecoveryClaimMode\"\n    },\n    \"savepointPath\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-jar-run-request-body-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JarRunRequestBody
---
