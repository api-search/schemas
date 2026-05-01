---
description: ResetJobBookmarkRequest schema from Amazon Glue API
layout: schema
name: ResetJobBookmarkRequest
properties_list:
- description: ''
  name: JobName
  type: object
- description: ''
  name: RunId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-reset-job-bookmark-request-schema.json
slug: glue-reset-job-bookmark-request
source_filename: glue-reset-job-bookmark-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-reset-job-bookmark-request-schema.json\",\n  \"title\": \"ResetJobBookmarkRequest\",\n  \"description\": \"ResetJobBookmarkRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobName\"\n        },\n        {\n          \"description\": \"The name of the job in question.\"\n        }\n      ]\n    },\n    \"RunId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RunId\"\n        },\n        {\n          \"description\": \"The unique run identifier associated with this job run.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-reset-job-bookmark-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ResetJobBookmarkRequest
---
