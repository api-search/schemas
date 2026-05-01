---
description: UpdateMLTransformResponse schema from Amazon Glue API
layout: schema
name: UpdateMLTransformResponse
properties_list:
- description: ''
  name: TransformId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-update-ml-transform-response-schema.json
slug: glue-update-ml-transform-response
source_filename: glue-update-ml-transform-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-ml-transform-response-schema.json\",\n  \"title\": \"UpdateMLTransformResponse\",\n  \"description\": \"UpdateMLTransformResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier for the transform that was updated.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-update-ml-transform-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: UpdateMLTransformResponse
---
