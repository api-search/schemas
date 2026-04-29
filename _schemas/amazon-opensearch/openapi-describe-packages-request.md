---
description: Container for request parameters to <code> <a>DescribePackage</a> </code> operation.
layout: schema
name: DescribePackagesRequest
properties_list:
- description: ''
  name: Filters
  type: object
- description: ''
  name: MaxResults
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-packages-request-schema.json
slug: openapi-describe-packages-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-request-schema.json\",\n  \"title\": \"DescribePackagesRequest\",\n  \"description\": \" Container for request parameters to <code> <a>DescribePackage</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Filters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribePackagesFilterList\"\n        },\n        {\n          \"description\": \"Only returns packages that match the <code>DescribePackagesFilterList</code> values.\"\n        }\n      ]\n    },\n    \"MaxResults\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaxResults\"\n        },\n        {\n          \"description\": \"Limits results to a maximum number of packages.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"Used for pagination. Only necessary if a previous API call includes a non-null NextToken value. If provided, returns results for the next page.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-request-schema.json
tags:
- Analytics
- AWS
- Elasticsearch
- Search
title: DescribePackagesRequest
---
