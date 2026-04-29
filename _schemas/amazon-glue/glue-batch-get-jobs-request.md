---
description: BatchGetJobsRequest schema from Amazon Glue API
layout: schema
name: BatchGetJobsRequest
properties_list:
- description: ''
  name: JobNames
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-jobs-request-schema.json
slug: glue-batch-get-jobs-request
source_filename: glue-batch-get-jobs-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-jobs-request-schema.json\",\n  \"title\": \"BatchGetJobsRequest\",\n  \"description\": \"BatchGetJobsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobNameList\"\n        },\n        {\n          \"description\": \"A list of job names, which might be the names returned from the <code>ListJobs</code> operation.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobNames\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-jobs-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetJobsRequest
---
