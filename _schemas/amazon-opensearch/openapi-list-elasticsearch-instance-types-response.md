---
description: Container for the parameters returned by <code> <a>ListElasticsearchInstanceTypes</a> </code> operation.
layout: schema
name: ListElasticsearchInstanceTypesResponse
properties_list:
- description: ''
  name: ElasticsearchInstanceTypes
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-list-elasticsearch-instance-types-response-schema.json
slug: openapi-list-elasticsearch-instance-types-response
source_filename: openapi-list-elasticsearch-instance-types-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-elasticsearch-instance-types-response-schema.json\",\n  \"title\": \"ListElasticsearchInstanceTypesResponse\",\n  \"description\": \" Container for the parameters returned by <code> <a>ListElasticsearchInstanceTypes</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ElasticsearchInstanceTypes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ElasticsearchInstanceTypeList\"\n        },\n        {\n          \"description\": \" List of instance types supported by Amazon Elasticsearch service for given <code> <a>ElasticsearchVersion</a> </code> \"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\":\
  \ \"In case if there are more results available NextToken would be present, make further request to the same API with received NextToken to paginate remaining results. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-list-elasticsearch-instance-types-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: ListElasticsearchInstanceTypesResponse
---
