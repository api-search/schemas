---
description: The details that define an aggregation based on operating system package type.
layout: schema
name: PackageAggregation
properties_list:
- description: ''
  name: packageNames
  type: object
- description: ''
  name: sortBy
  type: object
- description: ''
  name: sortOrder
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-package-aggregation-schema.json
slug: inspector-package-aggregation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-aggregation-schema.json\",\n  \"title\": \"PackageAggregation\",\n  \"description\": \"The details that define an aggregation based on operating system package type.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"packageNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StringFilterList\"\n        },\n        {\n          \"description\": \"The names of packages to aggregate findings on.\"\n        }\n      ]\n    },\n    \"sortBy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PackageSortBy\"\n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    },\n    \"sortOrder\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SortOrder\"\
  \n        },\n        {\n          \"description\": \"The order to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-aggregation-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: PackageAggregation
---
