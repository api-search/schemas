---
description: A response that contains details on the results of a finding aggregation by title.
layout: schema
name: TitleAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: severityCounts
  type: object
- description: ''
  name: title
  type: object
- description: ''
  name: vulnerabilityId
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-title-aggregation-response-schema.json
slug: inspector-title-aggregation-response
source_filename: inspector-title-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-title-aggregation-response-schema.json\",\n  \"title\": \"TitleAggregationResponse\",\n  \"description\": \"A response that contains details on the results of a finding aggregation by title.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The ID of the Amazon Web Services account associated with the findings.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"An object that represent the count of matched findings per severity.\"\n        }\n      ]\n    },\n    \"title\": {\n      \"\
  allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The title that the findings were aggregated on.\"\n        }\n      ]\n    },\n    \"vulnerabilityId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The vulnerability ID of the finding.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"title\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-title-aggregation-response-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: TitleAggregationResponse
---
