---
description: BatchGetJobsResponse schema from Amazon Glue API
layout: schema
name: BatchGetJobsResponse
properties_list:
- description: ''
  name: Jobs
  type: object
- description: ''
  name: JobsNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-jobs-response-schema.json
slug: glue-batch-get-jobs-response
source_filename: glue-batch-get-jobs-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-jobs-response-schema.json\",\n  \"title\": \"BatchGetJobsResponse\",\n  \"description\": \"BatchGetJobsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Jobs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobList\"\n        },\n        {\n          \"description\": \"A list of job definitions.\"\n        }\n      ]\n    },\n    \"JobsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobNameList\"\n        },\n        {\n          \"description\": \"A list of names of jobs not found.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-jobs-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetJobsResponse
---
