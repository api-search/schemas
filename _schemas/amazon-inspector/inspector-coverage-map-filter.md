---
description: Contains details of a coverage map filter.
layout: schema
name: CoverageMapFilter
properties_list:
- description: ''
  name: comparison
  type: object
- description: ''
  name: key
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-coverage-map-filter-schema.json
slug: inspector-coverage-map-filter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-map-filter-schema.json\",\n  \"title\": \"CoverageMapFilter\",\n  \"description\": \"Contains details of a coverage map filter.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"comparison\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CoverageMapComparison\"\n        },\n        {\n          \"description\": \"The operator to compare coverage on.\"\n        }\n      ]\n    },\n    \"key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The tag key associated with the coverage map filter.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n      \
  \  {\n          \"description\": \"The tag value associated with the coverage map filter.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"comparison\",\n    \"key\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-coverage-map-filter-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: CoverageMapFilter
---
