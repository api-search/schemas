---
description: JobDetails schema from Apache Flink REST API
layout: schema
name: JobDetails
properties_list:
- description: ''
  name: duration
  type: integer
- description: ''
  name: end-time
  type: integer
- description: ''
  name: jid
  type: object
- description: ''
  name: last-modification
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: pending-operators
  type: integer
- description: ''
  name: start-time
  type: integer
- description: ''
  name: state
  type: object
- description: ''
  name: tasks
  type: object
provider_name: Apache Flink
provider_slug: apache-flink
schema_file: json-schema/flink-rest-job-details-schema.json
slug: flink-rest-job-details
source_filename: flink-rest-job-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-schema.json\",\n  \"title\": \"JobDetails\",\n  \"description\": \"JobDetails schema from Apache Flink REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"duration\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"end-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"jid\": {\n      \"$ref\": \"#/components/schemas/JobID\"\n    },\n    \"last-modification\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"pending-operators\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"start-time\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"state\": {\n      \"$ref\": \"#/components/schemas/JobStatus\"\
  \n    },\n    \"tasks\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"integer\",\n        \"format\": \"int32\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-flink/refs/heads/main/json-schema/flink-rest-job-details-schema.json
tags:
- Apache
- Batch Processing
- Big Data
- Open Source
- Real-Time Analytics
- Stateful Computing
- Stream Processing
title: JobDetails
---
