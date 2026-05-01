---
description: BatchGetAccountStatusRequest schema
layout: schema
name: BatchGetAccountStatusRequest
properties_list:
- description: ''
  name: accountIds
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-account-status-request-schema.json
slug: inspector-batch-get-account-status-request
source_filename: inspector-batch-get-account-status-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-account-status-request-schema.json\",\n  \"title\": \"BatchGetAccountStatusRequest\",\n  \"description\": \"BatchGetAccountStatusRequest schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountIdSet\"\n        },\n        {\n          \"description\": \"The 12-digit Amazon Web Services account IDs of the accounts to retrieve Amazon Inspector status for.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-account-status-request-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetAccountStatusRequest
---
