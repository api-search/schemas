---
description: GetUserDefinedFunctionResponse schema from Amazon Glue API
layout: schema
name: GetUserDefinedFunctionResponse
properties_list:
- description: ''
  name: UserDefinedFunction
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-user-defined-function-response-schema.json
slug: glue-get-user-defined-function-response
source_filename: glue-get-user-defined-function-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-user-defined-function-response-schema.json\",\n  \"title\": \"GetUserDefinedFunctionResponse\",\n  \"description\": \"GetUserDefinedFunctionResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UserDefinedFunction\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UserDefinedFunction\"\n        },\n        {\n          \"description\": \"The requested function definition.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-user-defined-function-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetUserDefinedFunctionResponse
---
