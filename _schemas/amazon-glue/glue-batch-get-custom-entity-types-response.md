---
description: BatchGetCustomEntityTypesResponse schema from Amazon Glue API
layout: schema
name: BatchGetCustomEntityTypesResponse
properties_list:
- description: ''
  name: CustomEntityTypes
  type: object
- description: ''
  name: CustomEntityTypesNotFound
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-batch-get-custom-entity-types-response-schema.json
slug: glue-batch-get-custom-entity-types-response
source_filename: glue-batch-get-custom-entity-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-custom-entity-types-response-schema.json\",\n  \"title\": \"BatchGetCustomEntityTypesResponse\",\n  \"description\": \"BatchGetCustomEntityTypesResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CustomEntityTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEntityTypes\"\n        },\n        {\n          \"description\": \"A list of <code>CustomEntityType</code> objects representing the custom patterns that have been created.\"\n        }\n      ]\n    },\n    \"CustomEntityTypesNotFound\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomEntityTypeNames\"\n        },\n        {\n          \"description\": \"A list of the names of custom patterns that were not found.\"\n     \
  \   }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-batch-get-custom-entity-types-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: BatchGetCustomEntityTypesResponse
---
