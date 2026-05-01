---
description: CreateMLTransformResponse schema from Amazon Glue API
layout: schema
name: CreateMLTransformResponse
properties_list:
- description: ''
  name: TransformId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-create-ml-transform-response-schema.json
slug: glue-create-ml-transform-response
source_filename: glue-create-ml-transform-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-ml-transform-response-schema.json\",\n  \"title\": \"CreateMLTransformResponse\",\n  \"description\": \"CreateMLTransformResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"A unique identifier that is generated for the transform.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-create-ml-transform-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: CreateMLTransformResponse
---
