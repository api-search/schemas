---
description: UpdateJobRequest schema from Amazon Glue API
layout: schema
name: UpdateJobRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: JobUpdate
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-job-request-schema.json
slug: glue-update-job-request
source_filename: glue-update-job-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-request-schema.json\",\n  \"title\": \"UpdateJobRequest\",\n  \"description\": \"UpdateJobRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"The name of the job definition to update.\"\n        }\n      ]\n    },\n    \"JobUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobUpdate\"\n        },\n        {\n          \"description\": \"Specifies the values with which to update the job definition. Unspecified configuration is removed or reset to default values.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\",\n    \"JobUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateJobRequest
---
