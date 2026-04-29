---
description: BatchGetDataQualityResultResponse schema from Amazon Glue API
layout: schema
name: BatchGetDataQualityResultResponse
properties_list:
- description: ''
  name: Results
  type: object
- description: ''
  name: ResultsNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-data-quality-result-response-schema.json
slug: glue-batch-get-data-quality-result-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-data-quality-result-response-schema.json\",\n  \"title\": \"BatchGetDataQualityResultResponse\",\n  \"description\": \"BatchGetDataQualityResultResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Results\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityResultsList\"\n        },\n        {\n          \"description\": \"A list of <code>DataQualityResult</code> objects representing the data quality results.\"\n        }\n      ]\n    },\n    \"ResultsNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DataQualityResultIds\"\n        },\n        {\n          \"description\": \"A list of result IDs for which results were not found.\"\n        }\n      ]\n    }\n  },\n  \"required\"\
  : [\n    \"Results\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-data-quality-result-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetDataQualityResultResponse
---
