---
description: BatchGetAccountStatusResponse schema
layout: schema
name: BatchGetAccountStatusResponse
properties_list:
- description: ''
  name: accounts
  type: object
- description: ''
  name: failedAccounts
  type: object
provider_name: Amazon Inspector
provider_slug: amazon-inspector
schema_file: json-schema/inspector-batch-get-account-status-response-schema.json
slug: inspector-batch-get-account-status-response
source_filename: inspector-batch-get-account-status-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-account-status-response-schema.json\",\n  \"title\": \"BatchGetAccountStatusResponse\",\n  \"description\": \"BatchGetAccountStatusResponse schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AccountStateList\"\n        },\n        {\n          \"description\": \"An array of objects that provide details on the status of Amazon Inspector for each of the requested accounts.\"\n        }\n      ]\n    },\n    \"failedAccounts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FailedAccountList\"\n        },\n        {\n          \"description\": \"An array of objects detailing any accounts that failed to enable Amazon Inspector and why.\"\n        }\n      ]\n\
  \    }\n  },\n  \"required\": [\n    \"accounts\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-inspector/refs/heads/main/json-schema/inspector-batch-get-account-status-response-schema.json
tags:
- Compliance
- Container Security
- EC2
- Lambda
- Security
- Vulnerability Scanning
title: BatchGetAccountStatusResponse
---
