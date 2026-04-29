---
description: GetMLTransformsRequest schema from Amazon Glue API
layout: schema
name: GetMLTransformsRequest
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: Filter
  type: object
- description: ''
  name: Sort
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-get-ml-transforms-request-schema.json
slug: glue-get-ml-transforms-request
source_filename: glue-get-ml-transforms-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transforms-request-schema.json\",\n  \"title\": \"GetMLTransformsRequest\",\n  \"description\": \"GetMLTransformsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A paginated token to offset the results.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum number of results to return.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformFilterCriteria\"\n        },\n \
  \       {\n          \"description\": \"The filter transformation criteria.\"\n        }\n      ]\n    },\n    \"Sort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformSortCriteria\"\n        },\n        {\n          \"description\": \"The sorting criteria.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-get-ml-transforms-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: GetMLTransformsRequest
---
