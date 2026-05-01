---
description: GetPlanResponse schema from Amazon Glue API
layout: schema
name: GetPlanResponse
properties_list:
- description: ''
  name: PythonScript
  type: object
- description: ''
  name: ScalaCode
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-plan-response-schema.json
slug: glue-get-plan-response
source_filename: glue-get-plan-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-plan-response-schema.json\",\n  \"title\": \"GetPlanResponse\",\n  \"description\": \"GetPlanResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PythonScript\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PythonScript\"\n        },\n        {\n          \"description\": \"A Python script to perform the mapping.\"\n        }\n      ]\n    },\n    \"ScalaCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScalaCode\"\n        },\n        {\n          \"description\": \"The Scala code to perform the mapping.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-plan-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetPlanResponse
---
