---
description: GetJobResponse schema from Amazon Glue API
layout: schema
name: GetJobResponse
properties_list:
- description: ''
  name: Job
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-job-response-schema.json
slug: glue-get-job-response
source_filename: glue-get-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-response-schema.json\",\n  \"title\": \"GetJobResponse\",\n  \"description\": \"GetJobResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Job\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Job\"\n        },\n        {\n          \"description\": \"The requested job definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetJobResponse
---
