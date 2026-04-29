---
description: BatchGetDataQualityResultRequest schema from Amazon Glue API
layout: schema
name: BatchGetDataQualityResultRequest
properties_list:
- description: ''
  name: ResultIds
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-data-quality-result-request-schema.json
slug: glue-batch-get-data-quality-result-request
source_filename: glue-batch-get-data-quality-result-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-data-quality-result-request-schema.json\",\n  \"title\": \"BatchGetDataQualityResultRequest\",\n  \"description\": \"BatchGetDataQualityResultRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResultIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityResultIds\"\n        },\n        {\n          \"description\": \"A list of unique result IDs for the data quality results.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResultIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-data-quality-result-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetDataQualityResultRequest
---
