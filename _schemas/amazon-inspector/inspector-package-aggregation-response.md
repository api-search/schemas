---
description: A response that contains the results of a finding aggregation by image layer.
layout: schema
name: PackageAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: packageName
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-package-aggregation-response-schema.json
slug: inspector-package-aggregation-response
source_filename: inspector-package-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-aggregation-response-schema.json\",\n  \"title\": \"PackageAggregationResponse\",\n  \"description\": \"A response that contains the results of a finding aggregation by image layer.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account associated with the findings.\"\n        }\n      ]\n    },\n    \"packageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the operating system package.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"An object that contains the count of matched findings per severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"packageName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-package-aggregation-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: PackageAggregationResponse
---
