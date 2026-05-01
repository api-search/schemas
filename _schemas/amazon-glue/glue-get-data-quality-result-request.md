---
description: GetDataQualityResultRequest schema from Amazon Glue API
layout: schema
name: GetDataQualityResultRequest
properties_list:
- description: ''
  name: ResultId
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-data-quality-result-request-schema.json
slug: glue-get-data-quality-result-request
source_filename: glue-get-data-quality-result-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-result-request-schema.json\",\n  \"title\": \"GetDataQualityResultRequest\",\n  \"description\": \"GetDataQualityResultRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResultId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/HashString\"\n        },\n        {\n          \"description\": \"A unique result ID for the data quality result.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResultId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-data-quality-result-request-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetDataQualityResultRequest
---
