---
description: GetJobRunRequest schema from Amazon Glue API
layout: schema
name: GetJobRunRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: RunId
  type: object
- description: ''
  name: PredecessorsIncluded
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-job-run-request-schema.json
slug: glue-get-job-run-request
source_filename: glue-get-job-run-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-run-request-schema.json\",\n  \"title\": \"GetJobRunRequest\",\n  \"description\": \"GetJobRunRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Name of the job definition being run.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdString\"\n        },\n        {\n          \"description\": \"The ID of the job run.\"\n        }\n      ]\n    },\n    \"PredecessorsIncluded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BooleanValue\"\n        },\n        {\n          \"description\": \"True if a\
  \ list of predecessor runs should be returned.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\",\n    \"RunId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-run-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetJobRunRequest
---
