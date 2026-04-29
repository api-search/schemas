---
description: ListMLTransformsRequest schema from Amazon Glue API
layout: schema
name: ListMLTransformsRequest
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
- description: ''
  name: Tags
  type: object
provider_name: Amazon Glue
provider_slug: amazon-glue
schema_file: json-schema/glue-list-ml-transforms-request-schema.json
slug: glue-list-ml-transforms-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-ml-transforms-request-schema.json\",\n  \"title\": \"ListMLTransformsRequest\",\n  \"description\": \"ListMLTransformsRequest schema from Amazon Glue API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PaginationToken\"\n        },\n        {\n          \"description\": \"A continuation token, if this is a continuation request.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PageSize\"\n        },\n        {\n          \"description\": \"The maximum size of a list to return.\"\n        }\n      ]\n    },\n    \"Filter\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformFilterCriteria\"\
  \n        },\n        {\n          \"description\": \"A <code>TransformFilterCriteria</code> used to filter the machine learning transforms.\"\n        }\n      ]\n    },\n    \"Sort\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransformSortCriteria\"\n        },\n        {\n          \"description\": \"A <code>TransformSortCriteria</code> used to sort the machine learning transforms.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Specifies to return only these tagged resources.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-glue/refs/heads/main/json-schema/glue-list-ml-transforms-request-schema.json
tags:
- Analytics
- AWS
- Data Catalog
- Data Integration
- Data Pipeline
- ETL
- Serverless
title: ListMLTransformsRequest
---
