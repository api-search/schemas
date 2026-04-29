---
description: An aggregation of findings by Amazon Web Services account ID.
layout: schema
name: AccountAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-account-aggregation-response-schema.json
slug: inspector-account-aggregation-response
source_filename: inspector-account-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-aggregation-response-schema.json\",\n  \"title\": \"AccountAggregationResponse\",\n  \"description\": \"An aggregation of findings by Amazon Web Services account ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"The number of findings by severity.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-account-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AccountAggregationResponse
---
