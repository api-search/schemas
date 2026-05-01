---
description: Container for results from <code>DescribeReservedElasticsearchInstanceOfferings</code>
layout: schema
name: DescribeReservedElasticsearchInstanceOfferingsResponse
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: ReservedElasticsearchInstanceOfferings
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-reserved-elasticsearch-instance-offerings-response-schema.json
slug: openapi-describe-reserved-elasticsearch-instance-offerings-response
source_filename: openapi-describe-reserved-elasticsearch-instance-offerings-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-reserved-elasticsearch-instance-offerings-response-schema.json\",\n  \"title\": \"DescribeReservedElasticsearchInstanceOfferingsResponse\",\n  \"description\": \"Container for results from <code>DescribeReservedElasticsearchInstanceOfferings</code>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Provides an identifier to allow retrieval of paginated results.\"\n        }\n      ]\n    },\n    \"ReservedElasticsearchInstanceOfferings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ReservedElasticsearchInstanceOfferingList\"\n        },\n        {\n          \"description\": \"List of reserved\
  \ Elasticsearch instance offerings\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-reserved-elasticsearch-instance-offerings-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribeReservedElasticsearchInstanceOfferingsResponse
---
