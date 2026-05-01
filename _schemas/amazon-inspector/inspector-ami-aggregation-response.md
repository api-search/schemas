---
description: A response that contains the results of a finding aggregation by AMI.
layout: schema
name: AmiAggregationResponse
properties_list:
- description: ''
  name: accountId
  type: object
- description: ''
  name: affectedInstances
  type: object
- description: ''
  name: ami
  type: object
- description: ''
  name: severityCounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-ami-aggregation-response-schema.json
slug: inspector-ami-aggregation-response
source_filename: inspector-ami-aggregation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ami-aggregation-response-schema.json\",\n  \"title\": \"AmiAggregationResponse\",\n  \"description\": \"A response that contains the results of a finding aggregation by AMI.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountId\"\n        },\n        {\n          \"description\": \"The Amazon Web Services account ID for the AMI.\"\n        }\n      ]\n    },\n    \"affectedInstances\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Long\"\n        },\n        {\n          \"description\": \"The IDs of Amazon EC2 instances using this AMI.\"\n        }\n      ]\n    },\n    \"ami\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmiId\"\
  \n        },\n        {\n          \"description\": \"The ID of the AMI that findings were aggregated for.\"\n        }\n      ]\n    },\n    \"severityCounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SeverityCounts\"\n        },\n        {\n          \"description\": \"An object that contains the count of matched findings per severity.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ami\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-ami-aggregation-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: AmiAggregationResponse
---
