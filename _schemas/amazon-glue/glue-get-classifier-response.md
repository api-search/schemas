---
description: GetClassifierResponse schema from Amazon Glue API
layout: schema
name: GetClassifierResponse
properties_list:
- description: ''
  name: Classifier
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-classifier-response-schema.json
slug: glue-get-classifier-response
source_filename: glue-get-classifier-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-classifier-response-schema.json\",\n  \"title\": \"GetClassifierResponse\",\n  \"description\": \"GetClassifierResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Classifier\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Classifier\"\n        },\n        {\n          \"description\": \"The requested classifier.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-classifier-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetClassifierResponse
---
