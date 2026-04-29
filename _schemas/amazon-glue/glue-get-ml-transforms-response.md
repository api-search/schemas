---
description: GetMLTransformsResponse schema from Amazon Glue API
layout: schema
name: GetMLTransformsResponse
properties_list:
- description: ''
  name: Transforms
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-transforms-response-schema.json
slug: glue-get-ml-transforms-response
source_filename: glue-get-ml-transforms-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transforms-response-schema.json\",\n  \"title\": \"GetMLTransformsResponse\",\n  \"description\": \"GetMLTransformsResponse schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Transforms\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformList\"\n        },\n        {\n          \"description\": \"A list of machine learning transforms.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A pagination token, if more results are available.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Transforms\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transforms-response-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTransformsResponse
---
