---
description: Container for response returned by <code> <a>DescribePackages</a> </code> operation.
layout: schema
name: DescribePackagesResponse
properties_list:
- description: ''
  name: PackageDetailsList
  type: object
- description: ''
  name: NextToken
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-packages-response-schema.json
slug: openapi-describe-packages-response
source_filename: openapi-describe-packages-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-response-schema.json\",\n  \"title\": \"DescribePackagesResponse\",\n  \"description\": \" Container for response returned by <code> <a>DescribePackages</a> </code> operation. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PackageDetailsList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageDetailsList\"\n        },\n        {\n          \"description\": \"List of <code>PackageDetails</code> objects.\"\n        }\n      ]\n    },\n    \"NextToken\": {\n      \"$ref\": \"#/components/schemas/String\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-response-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribePackagesResponse
---
