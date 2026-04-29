---
description: BatchDeleteTableVersionResponse schema from Amazon Glue API
layout: schema
name: BatchDeleteTableVersionResponse
properties_list:
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-delete-table-version-response-schema.json
slug: glue-batch-delete-table-version-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-version-response-schema.json\",\n  \"title\": \"BatchDeleteTableVersionResponse\",\n  \"description\": \"BatchDeleteTableVersionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TableVersionErrors\"\n        },\n        {\n          \"description\": \"A list of errors encountered while trying to delete the specified table versions.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-table-version-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchDeleteTableVersionResponse
---
