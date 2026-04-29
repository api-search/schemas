---
description: DeleteJobRequest schema from Amazon Glue API
layout: schema
name: DeleteJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-job-request-schema.json
slug: glue-delete-job-request
source_filename: glue-delete-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-job-request-schema.json\",\n  \"title\": \"DeleteJobRequest\",\n  \"description\": \"DeleteJobRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job definition to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-job-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteJobRequest
---
