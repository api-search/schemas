---
description: BatchGetCustomEntityTypesRequest schema from Amazon Glue API
layout: schema
name: BatchGetCustomEntityTypesRequest
properties_list:
- description: ''
  name: Names
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-custom-entity-types-request-schema.json
slug: glue-batch-get-custom-entity-types-request
source_filename: glue-batch-get-custom-entity-types-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-custom-entity-types-request-schema.json\",\n  \"title\": \"BatchGetCustomEntityTypesRequest\",\n  \"description\": \"BatchGetCustomEntityTypesRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Names\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEntityTypeNames\"\n        },\n        {\n          \"description\": \"A list of names of the custom patterns that you want to retrieve.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Names\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-custom-entity-types-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetCustomEntityTypesRequest
---
