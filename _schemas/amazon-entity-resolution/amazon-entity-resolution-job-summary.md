---
description: An object containing the <code>JobId</code>, <code>Status</code>, <code>StartTime</code>, and <code>EndTime</code> of a job.
layout: schema
name: JobSummary
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: jobId
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: status
  type: object
provider_name: Amazon Entity Resolution
provider_slug: amazon-entity-resolution
schema_file: json-schema/amazon-entity-resolution-job-summary-schema.json
slug: amazon-entity-resolution-job-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-job-summary-schema.json\",\n  \"title\": \"JobSummary\",\n  \"description\": \"An object containing the <code>JobId</code>, <code>Status</code>, <code>StartTime</code>, and <code>EndTime</code> of a job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time at which the job has finished.\"\n        }\n      ]\n    },\n    \"jobId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobId\"\n        },\n        {\n          \"description\": \"The ID of the job.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\
  \n        },\n        {\n          \"description\": \"The time at which the job was started.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobStatus\"\n        },\n        {\n          \"description\": \"The current status of the job. Either <code>running</code>, <code>succeeded</code>, <code>queued</code>, or <code>failed</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"jobId\",\n    \"startTime\",\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-entity-resolution/refs/heads/main/json-schema/amazon-entity-resolution-job-summary-schema.json
tags:
- Amazon Web Services
- AWS
- Data Integration
- Data Matching
- Entity Resolution
- Machine Learning
title: JobSummary
---
