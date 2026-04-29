---
description: BatchDeleteTableResponse schema from Amazon Glue API
layout: schema
name: BatchDeleteTableResponse
properties_list:
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-delete-table-response-schema.json
slug: glue-batch-delete-table-response
source_filename: glue-batch-delete-table-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-response-schema.json\",\n  \"title\": \"BatchDeleteTableResponse\",\n  \"description\": \"BatchDeleteTableResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableErrors\"\n        },\n        {\n          \"description\": \"A list of errors encountered in attempting to delete the specified tables.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchDeleteTableResponse
---
