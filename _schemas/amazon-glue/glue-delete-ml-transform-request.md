---
description: DeleteMLTransformRequest schema from Amazon Glue API
layout: schema
name: DeleteMLTransformRequest
properties_list:
- description: ''
  name: TransformId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-delete-ml-transform-request-schema.json
slug: glue-delete-ml-transform-request
source_filename: glue-delete-ml-transform-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-ml-transform-request-schema.json\",\n  \"title\": \"DeleteMLTransformRequest\",\n  \"description\": \"DeleteMLTransformRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"The unique identifier of the transform to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TransformId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-delete-ml-transform-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: DeleteMLTransformRequest
---
