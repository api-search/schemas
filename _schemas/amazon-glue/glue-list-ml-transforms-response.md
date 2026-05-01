---
description: ListMLTransformsResponse schema from Amazon Glue API
layout: schema
name: ListMLTransformsResponse
properties_list:
- description: ''
  name: TransformIds
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-ml-transforms-response-schema.json
slug: glue-list-ml-transforms-response
source_filename: glue-list-ml-transforms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-ml-transforms-response-schema.json\",\n  \"title\": \"ListMLTransformsResponse\",\n  \"description\": \"ListMLTransformsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TransformIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformIdList\"\n        },\n        {\n          \"description\": \"The identifiers of all the machine learning transforms in the account, or the machine learning transforms with the specified tags.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A continuation token, if the returned list does not contain the last metric available.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"TransformIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-ml-transforms-response-schema.json
tags:
- Analytics
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListMLTransformsResponse
---
