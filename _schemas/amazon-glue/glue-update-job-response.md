---
description: UpdateJobResponse schema from Amazon Glue API
layout: schema
name: UpdateJobResponse
properties_list:
- description: ''
  name: JobName
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-job-response-schema.json
slug: glue-update-job-response
source_filename: glue-update-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-response-schema.json\",\n  \"title\": \"UpdateJobResponse\",\n  \"description\": \"UpdateJobResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameString\"\n        },\n        {\n          \"description\": \"Returns the name of the updated job definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-job-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateJobResponse
---
