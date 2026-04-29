---
description: BatchGetFindingDetailsRequest schema
layout: schema
name: BatchGetFindingDetailsRequest
properties_list:
- description: ''
  name: findingArns
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-finding-details-request-schema.json
slug: inspector-batch-get-finding-details-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-finding-details-request-schema.json\",\n  \"title\": \"BatchGetFindingDetailsRequest\",\n  \"description\": \"BatchGetFindingDetailsRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"findingArns\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FindingArnList\"\n        },\n        {\n          \"description\": \"A list of finding ARNs.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"findingArns\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-finding-details-request-schema.json
tags:
- AWS
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetFindingDetailsRequest
---
