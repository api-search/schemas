---
description: Container for results from <code>DescribeReservedElasticsearchInstances</code>
layout: schema
name: DescribeReservedElasticsearchInstancesResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ReservedElasticsearchInstances
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-reserved-elasticsearch-instances-response-schema.json
slug: openapi-describe-reserved-elasticsearch-instances-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-reserved-elasticsearch-instances-response-schema.json\",\n  \"title\": \"DescribeReservedElasticsearchInstancesResponse\",\n  \"description\": \"Container for results from <code>DescribeReservedElasticsearchInstances</code>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Provides an identifier to allow retrieval of paginated results.\"\n        }\n      ]\n    },\n    \"ReservedElasticsearchInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservedElasticsearchInstanceList\"\n        },\n        {\n          \"description\": \"List of reserved Elasticsearch instances.\"\n        }\n    \
  \  ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-reserved-elasticsearch-instances-response-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribeReservedElasticsearchInstancesResponse
---
