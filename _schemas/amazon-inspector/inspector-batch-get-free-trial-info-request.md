---
description: BatchGetFreeTrialInfoRequest schema
layout: schema
name: BatchGetFreeTrialInfoRequest
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-free-trial-info-request-schema.json
slug: inspector-batch-get-free-trial-info-request
source_filename: inspector-batch-get-free-trial-info-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-free-trial-info-request-schema.json\",\n  \"title\": \"BatchGetFreeTrialInfoRequest\",\n  \"description\": \"BatchGetFreeTrialInfoRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchGetFreeTrialInfoRequestAccountIdsList\"\n        },\n        {\n          \"description\": \"The account IDs to get free trial status for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"accountIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-free-trial-info-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetFreeTrialInfoRequest
---
