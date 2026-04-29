---
description: A response that contains the results of a finding type aggregation.
layout: schema
name: FindingTypeAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-finding-type-aggregation-response-schema.json
slug: inspector-finding-type-aggregation-response
source_filename: inspector-finding-type-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-type-aggregation-response-schema.json\",\n  \"title\": \"FindingTypeAggregationResponse\",\n  \"description\": \"A response that contains the results of a finding type aggregation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account associated with the findings.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"The value to sort results by.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-finding-type-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: FindingTypeAggregationResponse
---
