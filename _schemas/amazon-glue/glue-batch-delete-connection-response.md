---
description: BatchDeleteConnectionResponse schema from Amazon Glue API
layout: schema
name: BatchDeleteConnectionResponse
properties_list:
- description: ''
  name: Succeeded
  type: object
- description: ''
  name: Errors
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-delete-connection-response-schema.json
slug: glue-batch-delete-connection-response
source_filename: glue-batch-delete-connection-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-connection-response-schema.json\",\n  \"title\": \"BatchDeleteConnectionResponse\",\n  \"description\": \"BatchDeleteConnectionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Succeeded\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NameStringList\"\n        },\n        {\n          \"description\": \"A list of names of the connection definitions that were successfully deleted.\"\n        }\n      ]\n    },\n    \"Errors\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorByName\"\n        },\n        {\n          \"description\": \"A map of the names of connections that were not successfully deleted to error details.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-delete-connection-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchDeleteConnectionResponse
---
