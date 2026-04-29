---
description: GetJobRequest schema from Amazon Glue API
layout: schema
name: GetJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-job-request-schema.json
slug: glue-get-job-request
source_filename: glue-get-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-request-schema.json\",\n  \"title\": \"GetJobRequest\",\n  \"description\": \"GetJobRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job definition to retrieve.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-job-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetJobRequest
---
