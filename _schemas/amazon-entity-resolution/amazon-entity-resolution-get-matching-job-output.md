---
description: GetMatchingJobOutput schema from AWS EntityResolution
layout: schema
name: GetMatchingJobOutput
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: errorDetails
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: metrics
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-get-matching-job-output-schema.json
slug: amazon-entity-resolution-get-matching-job-output
source_filename: amazon-entity-resolution-get-matching-job-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-matching-job-output-schema.json\",\n  \"title\": \"GetMatchingJobOutput\",\n  \"description\": \"GetMatchingJobOutput schema from AWS EntityResolution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the job has finished.\"\n        }\n      ]\n    },\n    \"errorDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorDetails\"\n        },\n        {\n          \"description\": \"An object containing an error message, if there was an error.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\
  \n        },\n        {\n          \"description\": \"The ID of the job.\"\n        }\n      ]\n    },\n    \"metrics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobMetrics\"\n        },\n        {\n          \"description\": \"Metrics associated with the execution, specifically total records processed, unique IDs generated, and records the execution skipped.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the job was started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The current status of the job. Either <code>running</code>, <code>succeeded</code>, <code>queued</code>, or <code>failed</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n\
  \    \"jobId\",\n    \"startTime\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-get-matching-job-output-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: GetMatchingJobOutput
---
