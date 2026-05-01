---
description: Filter to apply in <code>DescribePackage</code> response.
layout: schema
name: DescribePackagesFilter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon OpenSearch Service API
provider_slug: amazon-opensearch
schema_file: json-schema/openapi-describe-packages-filter-schema.json
slug: openapi-describe-packages-filter
source_filename: openapi-describe-packages-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-filter-schema.json\",\n  \"title\": \"DescribePackagesFilter\",\n  \"description\": \"Filter to apply in <code>DescribePackage</code> response.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribePackagesFilterName\"\n        },\n        {\n          \"description\": \"Any field from <code>PackageDetails</code>.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DescribePackagesFilterValues\"\n        },\n        {\n          \"description\": \"A non-empty list of values for the specified field.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-opensearch/refs/heads/main/json-schema/openapi-describe-packages-filter-schema.json
tags:
- Analytics
- Elasticsearch
- Search
title: DescribePackagesFilter
---
