---
description: ResetJobBookmarkResponse schema from Amazon Glue API
layout: schema
name: ResetJobBookmarkResponse
properties_list:
- description: ''
  name: JobBookmarkEntry
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-reset-job-bookmark-response-schema.json
slug: glue-reset-job-bookmark-response
source_filename: glue-reset-job-bookmark-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-reset-job-bookmark-response-schema.json\",\n  \"title\": \"ResetJobBookmarkResponse\",\n  \"description\": \"ResetJobBookmarkResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"JobBookmarkEntry\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JobBookmarkEntry\"\n        },\n        {\n          \"description\": \"The reset bookmark entry.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-reset-job-bookmark-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ResetJobBookmarkResponse
---
